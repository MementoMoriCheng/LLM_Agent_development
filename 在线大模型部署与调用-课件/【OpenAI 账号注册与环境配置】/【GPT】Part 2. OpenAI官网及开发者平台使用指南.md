




## OpenAI 官网使用指南



自 2023 年 2 月起，一款现象级产品 ChatGPT 传入国内，全球掀起了大模型技术的热潮，各种大模型持续迭代，为技术圈带来一波又一波的浪潮。截至目前，**OpenAI 基本奠定了大模型领域的领先地位**。虽然其他大模型在某些细分领域可能超过 GPT 系列模型，例如国外的 Claude、谷歌的 Gemini，以及国内的 GLM 等等，但从整体生态来看，**OpenAI 仍然是这场技术革命的霸主**。它拥有全球最全面的大模型生态体系、最强大的技术研发团队，以及最先进的大模型开发代码。

在本章中，我们将深入了解 OpenAI 的官网使用方法，帮助大家熟悉官方文档和开发者平台，为后续的大模型学习打下坚实基础。



### 课前须知



从本节开始，课程内容将进入技术的深水区，可能会出现一些新的名词和概念。但请大家不必担心，我们会用浅显易懂的语言，帮助不同技术层次的伙伴尽快掌握大模型的基础内容，让每个人都能跟上学习进度。

在正式开始本节内容之前，请确保完成以下准备工作：

- **准备一个可用的 OpenAI 账号 **，便于后续课程的学习（注册方法在前面邻近的课程内容里）。

- **掌握 Python 基础。** 后续课程会涉及大量的 Python 代码，掌握 Python 基础非常重要。如果还没有 Python 基础，可以参考加餐的《python基础系列课程》，重点掌握 Python 基础语法、函数编写。
---

在之前的课程视频中我们已经注册了OpenAI账号，所有服务（ChatGPT使用、Plus会员、API）都基于一个OpenAI账号，那么这3个主要的服务都有什么区别呢，我们为什么还有订阅ChatGPT Plus会员与注册ChatGPT API账户的教程呢？

1. **ChatGPT账号**
- **定义**：ChatGPT账号是用户访问OpenAI提供的ChatGPT服务所需的基本账户。通过注册一个OpenAI账号，用户可以免费使用ChatGPT的基础功能。
- **功能**：
  - 使用基础的ChatGPT对话功能。
  - 管理个人信息和设置。
  - 查看和管理对话历史记录。

 2.  **ChatGPT Plus 会员**

- **定义**：ChatGPT Plus 是 OpenAI 提供的付费服务，每月费用为 **20 美元**。**需用国外虚拟信用卡付款。**
- **优势**：
    
    1. **优先访问多种模型**：包括 **OpenAI o1-preview、o1-mini、GPT-4o、GPT-4o mini、GPT-4**，相比免费用户，Plus 会员有更多模型可用。
    2. **更多消息量**：可获得GPT-4o **5 倍的消息量**。
    3. **自定义 GPT**：支持创建和使用自定义的 GPT。
    
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241009163426.png)


### 3. ChatGPT API的充值
- **定义**：ChatGPT API是一种面向开发者的接口，允许将ChatGPT的语言模型功能集成到自己的应用、网站或服务中。
- **关系**：
  - **独立服务**：虽然ChatGPT API与个人ChatGPT账号相关联，但它是独立于ChatGPT Plus会员的服务。API的使用和收费方式与个人订阅不同。
  - **注册流程**：
    - **绑定付款的信用卡**：需先绑定虚拟信用卡充值后API才可被调用。
    - **获取API密钥**：注册后，开发者可以获取用于调用API的密钥。
    - **计费模式**：API使用通常基于调用次数或处理的字符数进行计费，与ChatGPT Plus的固定月费不同。
- **用途**：主要面向开发者和企业，允许在自己的产品或服务中嵌入ChatGPT的功能，例如聊天机器人、内容生成工具等。

### 三者关系总结
- **基础账号**：所有服务（ChatGPT使用、Plus会员、API）都基于一个OpenAI账号。
- **对话使用 vs 开发调用使用**：
  - **ChatGPT账号**和**ChatGPT Plus会员**主要面向个人用户，提供直接的对话体验和增强服务。
  - **ChatGPT API**面向开发者和企业，提供集成和定制化的解决方案。
- **收费模式**：
  - **ChatGPT账号**免费使用基础功能。
  - **ChatGPT Plus会员**采用订阅制，提供更优质的个人使用体验。需绑定虚拟信用卡付款。
  - **ChatGPT API**采用按使用量计费，适合不同规模的开发需求。需绑定信用卡付款。

使用场景：
- **个人用户小明**：
  - 注册一个ChatGPT账号，免费使用基础对话功能。
  - 觉得免费版响应速度慢或模型不够前沿，决定订阅ChatGPT Plus会员，享受更快的响应和优先服务。
  
- **开发者和大模型应用者小华**：
  - 使用个人的ChatGPT账号访问ChatGPT的对话功能。
  - 为了在自己开发的应用中集成ChatGPT功能，注册ChatGPT API，获取API密钥，并根据使用量支付费用。




## OpenAI 开发者平台概览



在技术学习的过程中，**官方文档是最权威、最全面的学习资料**。在 OpenAI 在线大模型的学习中，OpenAI 官网提供的官方教程是我们最好的学习文档。

OpenAI 官网主要展示公司的最新新闻、使命愿景、官方研究、大模型产品和开发者平台。官网地址是：https://openai.com/



![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011143233.png)



在 OpenAI 官网的所有信息中，**最重要的是开发者平台**。在接下来的学习中，开发者平台上的内容将成为你的“随身宝典”。无论遇到什么问题或有任何技术构想，都可以第一时间查看 OpenAI 的开发者平台。

开发者平台地址：https://platform.openai.com/



<center><img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241010193551.png" alt="OpenAI 开发者平台" /></center>



进入 OpenAI 开发者平台，可以看到主要有五个功能区：

1. **Documentation（文档）**
2. **API Reference（API 参考）**
3. **Playground（在线测试）**
4. **Dashboard（仪表盘）**
5. **Settings（设置）**

接下来，我们将介绍这些功能区，帮助大家熟悉 OpenAI 开发者平台的使用。

首先关于文档的内容主要分布在这两处：
**Documentation** 页面是专为使用 OpenAI 大模型设计的全面指南，旨在帮助用户从初学者到高级开发者全面掌握模型的各项功能与应用。
**API Reference** 页面是面向开发者的技术文档，详细介绍了 OpenAI 提供的各类 API 功能及其参数，帮助用户高效集成和应用这些接口。

### 1. Documentation：OpenAI 大模型使用指南



Documentation 页面地址：https://platform.openai.com/docs/overview

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011171443.png)



Documentation 页面信息非常丰富，**我们可以先看看 “Models” 页面**。在这个页面中，可以了解每类模型的具体介绍。再看看一些关键的功能点。

以 GPT-4 系列模型为例，我们可以清楚地看到：

- **可调用的具体模型**（例如 `gpt-4-0125-preview`）
- **每个模型的描述**（Description）
- **最大上下文长度**（Context Window）
- **预训练数据截止日期**（Training Data）

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011144847.png)


#### 关键概念：Tokens



在学习大模型时，理解 **Tokens** 的概念非常重要。

**什么是 Tokens？**

在大模型体系中，**Tokens 可以简单理解为文本的基本构建块**。类似于英语中的单词和标点符号，每个 Token 代表输入文本的一个元素。当我们向大模型输入一句话时，这句话会首先被分割成一系列 Tokens，模型根据这些 Tokens 来理解和处理你输入的文本信息。

**为什么要引入 Tokens 这个概念？**

主要原因是 **大模型无法直接理解原始文本**。将文本分割成 Tokens，可以将复杂的文本信息转换为计算机能够理解和处理的格式。这有助于模型捕捉词汇、语法和上下文之间的关系。

可以简单理解为：**Tokens 是连接人类语言和机器语言的桥梁**。

**Tokens 与文本之间如何转换？**

OpenAI 官方提供了一个工具 **Tokenizer**，可以测试任意输入的文本，并查看它们是如何被转换成 Tokens 的。

Tokenizer 工具地址：https://platform.openai.com/tokenizer

需要注意的是，不同语言转换成 Tokens 时，结果会有所不同。这是因为每种语言的结构、词汇和语法特点各异，导致分词规则和方法不同。一般来说，**1 个 Token 约等于 4 个英文字符**。

<center><img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241010191810.png" alt="Tokenizer 工具" /></center>



#### 最大上下文长度（Context Window）

回到模型的基本信息，**Context Window 表示每个模型的最大上下文长度**。对于 GPT-3.5 和 GPT-4 这类文本生成模型来说，**输入的提示语和模型生成的输出内容两部分加起来的总长度不能超过模型的最大上下文长度限制**。

例如，对于 `gpt-4-0125-preview` 模型来说，输入和输出加起来的总和不能超过 128K Tokens（相当于 200 页的 PDF 文档）。

<center><img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/image-20240312191143634.png" alt="模型上下文长度" style="zoom:80%;" /></center>



**为什么会有最大上下文长度限制？**

答案在于 “GPT” 的全称：**“Generative Pre-trained Transformer”**，即 **基于 Transformer 架构的生成式预训练模型**。

- **预训练（Pre-training）**：模型在大规模数据集上进行训练，学习语言的通用模式和结构。

- **生成式（Generative）**：模型有能力生成新的内容，根据之前的文本预测下一个词。

- **Transformer**：一种深度学习模型架构，特别适合处理序列数据，如文本。核心是自注意力（Self-Attention）机制，使模型在生成文本时考虑整个文本序列的上下文信息。

由于 GPT 模型在生成每个词时都会考虑之前的所有信息，为了平衡生成文本的质量、连贯性和计算资源的有效使用。所有大模型都有一个输入token的最大长度限制和输出token的最大长度限制。

其主要的功能点：

![300](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011154529.png)


2024年10月份OPENAI的开发者大会上，与去年的盛大的推出了这次，OpenAI没有发布重大产品，而是对现有的****AI****工具和****API****套件进行了渐进式改进。

他们公布了四项创新：**视觉微调 （Vision Fine-Tuning）、实时****API****（Realtime API）、模型蒸馏（Model Distillation）和提示缓存（Prompt Caching）。**

我们趁新发布抢先别人一步先了解一下他们，其详细的API调用与其余的功能都会在后续的课程中详细的讲解实战进行最佳实践。

-  视觉微调：多模态的定制化！

集大模型的文本微调开放以来，GPT-4o模型引入的视觉微调功能无疑是一项重大突破。开发者现在可以通过上传至少100张图像来优化模型的视觉任务表现。这项技术已在实际应用中展现出惊人的潜力，如在发布会上介绍的Grab公司利用它显著提高了地图服务的准确率，Automat公司则大幅提升了其自动化工具的成功率。视觉微调为自动驾驶、医学成像和视觉搜索等领域带来了革命性的可能。

![640.gif](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/640.gif)

- 实时API：实时语音到语音！

  AI客服成本已低至人工客服的一半，之前的AI客服系统通常需要经过这么几个步骤：
	1. 语音识别
	2. 文本推理
	3. 文本转语音

每个环节都可能引入误差，影响用户体验。但OpenAI的实时API直接实现了**语音到语音的转换**，省去了中间环节，大大提升了响应速度和准确性。

更厉害的是，这个API还支持**函数调用**。这意味着AI客服不仅能听懂你说什么，还能根据你的需求触发相应的操作，比如查询订单、修改信息等。

一个5分钟的AI客服通话只需0.75美元，折合下来每小时仅需9美元。
而美国一名人工客服的平均时薪是**15美元！**



- 模型蒸馏：大模型教小模型！

用"大厨级"的高级模型（比如o1-preview和GPT-4o）来指导"学徒级"的小模型（如GPT-4o mini）。
a. 记录大厨的每一步
b. 蒸馏
c. 评估表现结果

- 提示缓存：省钱！

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011160054.png)

同时值得一提的是类似的功能已经在Gemini、Claude以及Kimi等平台上线了～而OpenAI的区别在于它将这一过程自动化。

这意味着开发者无需手动配置或管理缓存，OpenAI的系统会智能地处理输入tokens的缓存和重用

### 2. API Reference：API 功能及参数详解


在 OpenAI 开发者平台上，**API Reference 页面** 通过详尽的功能描述和参数说明，为开发者提供了全面的技术支持，确保能够高效、准确地集成和利用 OpenAI 的各类 API 功能。对于我们的学习来说，这个页面非常重要。后续需要经常回到这个页面查看。

API Reference 页面地址：https://platform.openai.com/docs/api-reference/introduction

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011171654.png)




在这里，你可以找到每个 API 的详细说明，包括参数解释、使用示例等。这对于理解如何调用 API、设置参数，以及处理返回结果非常有帮助。



### 3. Playground和Dashboard：基于网页的模型调用和测试



OpenAI 官网提供了一个非常实用的工具：**Playground和Dashboard**。
Playground页面类似于一个在线的模型调用应用，允许我们直接在网页上选择不同类型的模型、调整参数、输入提示词，测试模型的输出结果。并且可以体验比对话页面更多的功能，例如TTS文字转语音以及刚才说的实时API语音到语音的功能。


Playground 页面地址：https://platform.openai.com/playground

<center><img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/image-20240313195646600.png" alt="Playground 页面" /></center>

- **只有充值了 ChatGPT API 的用户可以访问 ChatGPT Playground。我们会在下节课讲解充值ChatGPT API的流程。否则是发送不出去的，因为它其实是属于在调用ChatGPT API。

 ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011163038.png)


**Playground 的主要特点：**

- **无需编写代码**：可以直接与大模型交互，观察结果。输入提示后，模型会立即生成响应。
- **功能丰富**：有对话，TTS文字转语音以及实时API语音到语音等的功能
- **参数调节**：可以调整温度（temperature）、最大长度（max tokens）等参数，观察对结果的影响。

对于初学者来说，Playground 是一个非常好的实践平台。但是，需要对大模型的基本参数有所了解，才能充分利用这个工具。

Dashboard
通过 Dashboard，用户可以管理账户设置、查看使用统计、处理账单事务以及账户相关联的上传和管理用于微调的数据集存储，微调的模型，使用预定义指标进行评估等都在这里找到。
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011164910.png)



### 4. 费用和使用限制



由于 OpenAI 的在线大模型是通过个人 API-Key 验证的方式，向 OpenAI 的线上模型提交计算请求，并实时获取返回结果。在实际调用中，会根据调用的模型类型、调用次数、输入和输出文本的数量进行计费。**因此，我们需要时刻关注费用支出情况。**

自 2023 年以来，OpenAI 的商用模型价格已经下降了十几次。

比如，当 2023 年 3 月发布的 GPT-4 还要每百万个输入 Token 收费 30 美元时，现如今，GPT-4o 版本的费用已经下降到每百万个输入 2.5 美元。

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011150503.png)

这一价格降幅达到了惊人的 91%！这种大幅度降价让更多企业能够负担得起，正是 OpenAI 让 AI 普及的重要推动力。也不禁想象OpenAI 首席执行官 Sam Altman 对 AI 的愿景：让 AI 像电力一样无处不在。的蓝图实现的世界。

**计费规则**

具体的计费规则可以在 **Pricing** 页面查看：https://openai.com/pricing

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011160054.png)


对于个人学习或练习，可以先使用mini的 API。



**调用限制**

在调用 API 的过程中，为了保护计算资源，OpenAI 对各模型的 API 设置了每分钟请求最大次数（RPM：Requests Per Minute）、每天最大请求次数（RPD：Requests Per Day）、每分钟 Token 通信量最大值（TPM：Tokens Per Minute）等限制。

这些限制可以在个人中心的 **Rate Limits** 页面查看：https://platform.openai.com/account/rate-limits

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20241011171850.png)


注意：这些限制与账号等级有关，不同等级对应的条件和限制可以在此页面查看：https://platform.openai.com/docs/guides/rate-limits/usage-tiers

**账户余额和使用情况**

我们需要时刻关注账户余额和当前的使用金额。可以在个人中心的 **Usage** 页面查看账户余额，以及过去一段时间的消费情况：https://platform.openai.com/account/usage

<center><img src="https://snowball101.oss-cn-beijing.aliyuncs.com/img/202402271816788.png" alt="Usage 页面" style="zoom:80%;" /></center>

另外，可以在 **Billing** -> **Usage Limits** 页面设置每个月的最大消费总金额，默认为 120 美元。如果当月 API 使用金额超过该限制，OpenAI 会停止对该 API Key 的响应。这个设置可以有效防止由于 API 滥用导致的费用超支。

Usage Limits 页面地址：https://platform.openai.com/account/billing/limits

<center><img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/image-20240313202134441.png" alt="Usage Limits 页面" /></center>


看了这么多，小伙伴们是不是准备好进行API的开通充值了呢，接下来就让我们准备好迈进API的大门吧
---



