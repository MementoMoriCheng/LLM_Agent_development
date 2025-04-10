官方用一句话介绍这个命名：“resetting the counter back to 1.”

新 o1 模型中的推理是如何工作的呢？
- 关键点是推理使模型能够在生成最终响应之前考虑多种方法。 
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241022192433.png)
🧠 OpenAI 引入了推理令牌，以便在响应之前“思考”。这些令牌分解提示并考虑多种方法。 

过程： 
1. 生成推理令牌
2. 产生可见的完成令牌作为答案 
3. 从上下文中丢弃推理标记  丢弃推理标记使上下文专注于关键信息 

多步骤对话流程： 
-  输入和输出的令牌在回合之间传递 
- 推理令牌在每个回合后被丢弃 
上下文窗口：128k 令牌 

OpenAI Strawberry (o1) 的发布标志着推理时扩展（inference-time scaling）这一范式在生产环境中的普及和部署

之前的LLM与o1的时间分配：
1. Pre-training (预训练阶段) 
2. Post-training (后训练阶段) 
3. Inference (推理阶段) 
![image](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/28777116_249bd793-3578-4a05-874a-bf391f1b3abd.png)

- 学习：通过增加训练数据和计算量来提升模型的内在能力，即预训练和后训练，这是之前大模型的主要路线。
- 实时推理：在推理时，不仅是在给出答案，而是会深入思考“为什么这个答案是正确的”。这和我们平时做数学题或解答问题时的过程类似：我们先思考，再得出结论。。且单纯依赖预训练，模型可能无法实现高级推理能力，尤其是在推理需要超越算力和数据的复杂情况下。

思考未来
- 实时搜索推理：在推理阶段通过搜索来扩展模型的能力边界，可以实时利用外部工具知识和计算资源（听起来是不是就有点像之前开发者在做的Agent）。

大模型发展的一个重要转折点：从纯粹依赖预训练向"预训练+后训练推理"的混合模式转变。

1. 知识与推理的分离：
- 现状：大模型参数大量用于存储事实知识
- 新思路：抽取出一个精简的"推理核心"
  * 负责逻辑推理能力
  * 会调用外部工具（浏览器、代码验证器等）
  * 可以显著减少模型参数量

2. 计算资源分配的转变：
- 从：大量计算用于预训练/后训练
- 到：将计算资源转移到实时推理阶段
	类似AlphaGo的MCTS
	  * 在模拟空间中探索不同策略
	  * 通过多次模拟找到最优解
	  * 可以动态调整搜索深度和广度

3 . 技术路线：
- 构建轻量级推理核心，CoT 虽然也能生成中间推理步骤，但没有教会模型"如何从内部深入思考问题的关联"，可能通过 Bootstrap 方式生成推理过程(Rationales)  融入到训练这个推理核心过程中。
- 将推理过程融入到训练过程中，让模型学会进行推理
- 开发高效的工具调用接口
- 设计推理阶段的智能的搜索策略， 优化实时推理的性能
	1. 基于预训练的大语言模型。
	2. 利用 RL 和树搜索等方法引导模型生成合理的推理过程。
	3. 将推理过程转化为细粒度的奖励信号（token级别，句子级别的节点），用于模型训练。
	4. 通过自举生成新的高真值数据，并利用这些数据进一步提升模型能力。
未来思考方向：怎么去平衡训练阶段和推理阶段的算力，从而总体达到最好的效果，也就是在推理搜索部分做出一些优化。

o1现状：
o1 在多个领域展现出卓越的性能，包括：在编程竞赛（Codeforces）中排名前 89%，在美国数学奥林匹克竞赛（AIME）资格赛中排名前 500，在物理、生物和化学问题基准测试（GPQA）中超越了人类博士水平的准确性。虽然 o1 的易用性仍在改进中，但 OpenAI 已发布早期预览版 o1-preview，供 ChatGPT 和受信任的 API 用户使用。

o1 的性能提升得益于大规模强化学习算法和更长的“思考”时间（测试时计算）。o1 在各种推理任务上的表现明显优于 GPT-4o，在许多基准测试中甚至能与人类专家匹敌。例如，o1 在 AIME 竞赛中取得了接近前 500 名学生的成绩，并在 GPQA Diamond 基准测试中超越了人类博士的准确性。在编程方面，经过微调的 o1 模型在国际信息学奥林匹克竞赛（IOI）中排名前 49%。
o1 使用“思维链”进行推理，强化学习帮助其改进思维过程、识别和纠正错误，并尝试不同的方法。虽然“思维链”对模型的安全性和一致性至关重要，但出于用户体验、竞争优势和监控等多方面考虑，o1-preview 向用户展示的是“思维链”的总结，而非原始的思维过程。
虽然在数据分析、编码和数学等推理密集型任务中，o1-preview 比 GPT-4o 更受人类青睐，但在某些自然语言任务上表现不佳。
https://openai.com/index/learning-to-reason-with-llms/


o1使用路径与API调用价格与限制：
- 如果您有 ChatGPT Plus 或 ChatGPT Team 帐户，则可以在页面顶部的模型选择器中选择 o1-preview 或 o1-mini。
- 可以使用 OpenAI o1-preview 每周访问 50 条消息，使用 OpenAI o1-mini 开始每天可以访问 50 条消息。（在更新）
[![](https://openai.intercom-attachments-7.com/i/o/1177121834/dda6db9b1fb94642b0f5b94c/AD_4nXfLLU0tv8mRZO5wJMUpwmnhOFC3uPEa-BmDrmE6dRr5QtxaS17EU8OhrtiX9oSnWeODsa6DbXtDdSvyCXS0lswvAkWD8MXaMAtRJp-fplt26LWc_qmHZu_SApb0eiTsO_nUS-aEdkBUTCLI-7Cvcg6avez2?expires=1729596600&signature=7f86fec4749a5de16d4db5ca9f6e93a87d6351fc4bdb3c7249061d7e95b9bc37&req=dSEgEch8nIlcXfMW1HO4zb0C%2FmKP%2BImF%2B%2FrIh%2BMvSLy7MZFf1xRb9bv1znGa%0A6kgLWoK72w%2FD3pD4dCM%3D%0A)
如果使用API则需要个人用户到达3级，但他会更新：
https://platform.openai.com/docs/guides/rate-limits/usage-tiers?context=tier-free

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241025150051.png)

https://help.openai.com/en/articles/9824962-openai-o1-preview-and-o1-mini-usage-limits-on-chatgpt-and-the-api