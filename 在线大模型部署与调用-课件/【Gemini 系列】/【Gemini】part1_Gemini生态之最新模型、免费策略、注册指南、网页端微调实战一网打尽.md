Gemini系列模型：
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240910154618.png)

从两个最新版本的大模型介绍Gemini生态：
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919105545.png)

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918120217.png)
注册了Gemini，你将可以不用绑定信用卡免费使用最智能大模型！免费体验微调！免费调用API！免费尝试音视频多模态！
## Gemini 1.5 Flash 和 Gemini 1.5 Pro 免费层级的价格  

| 功能               | Gemini 1.5 Flash              | Gemini 1.5 Pro            |     |
| ---------------- | ----------------------------- | ------------------------- | --- |
| 模型               | Gemini 1.5 Flash              | Gemini 1.5 Pro            |     |
| 特点               | 最快的多模态模型，处理重复性任务出色，100万个上下文窗口 | 新一代模型，突破性的 200 万上下文窗口     |     |
| 发布状态             | 正式推出，可用于生产环境                  | 正式推出，可用于生产环境              |     |
| **免费层级**         |                               |                           |     |
| API 服务           | 通过 API 服务提供，速率限制较低，用于测试目的     | 通过 API 服务提供，速率限制较低，用于测试目的 |     |
| Google AI Studio | 在所有适用的国家/地区完全免费               | 在所有适用的国家/地区完全免费           |     |
| **速率限制**         |                               |                           |     |
| 每分钟请求数 (RPM)     | 15                            | 2                         |     |
| 每分钟token数 (TPM)  | 1,000,000                     | 32,000                    |     |
| 每日请求数 (RPD)      | 1,500                         | 50                        |     |
| **价格**           |                               |                           |     |
| 输入价格             | 免费                            | 免费                        |     |
| 输出价格             | 免费                            | 免费                        |     |
| **上下文缓存**        |                               |                           |     |
| 存储               | 免费，每小时最多 100 万个令牌存储           | 不适用                       |     |

* Gemini 1.5 Flash 更适合需要高吞吐量和较大上下文窗口（100 万）的任务，例如处理重复性任务。  
* Gemini 1.5 Pro 提供更大的上下文窗口（200 万），但免费层级的速率限制较低。它更适合需要处理更长文本或对话的场景，但目前不支持调整和上下文缓存。


# Gemini的注册流程

Gemini相关产品，如web端页面，AI studio等都是谷歌的产品，登录也是用谷歌账号登录。可以说，Gemini的注册实际上就是Google账号的注册。

## Gemini注册流程图

## 注册主要门槛：接收国外手机号证码

在Google账号的注册过程中，Google账号的手机号验证可能要涉及到接收国外手机号的验证码。此时我们就需要使用**虚拟号码**来通过验证。

一种方法是下面教程用的——需要借助老牌的主流的 **SMS接码平台“SMS-active”** 提供的不同服务，不同国家的短信虚拟号码来绕过地理限制接受验证码。

因为不同服务的，不同国家的虚拟号码都有一定的价格，所以在购买前要先最低预充值2美金，折合人民币不到15元，几乎所有的SMS接码平台都需要先充值再购买。而在具体的使用时，我们大概需要花0.5美金的点数（折合人民币最多2元），剩下的都可以留着购买其他国外服务的手机号或帮助朋友注册。

另一种方法则可以在某宝上进行购买，搜索“SMS虚拟手机号”，联系客服告知我们要注册的是什么服务，即谷歌账号，并不直接是Gemini，接下来客服会发给我们验证码，其实商家就是用第一种方法再卖给我们。
注意，页面价格不一定为实际价格，合理价格在1~5元以内，如果选择英美地区会更贵一些。

建议掌握SMS-active平台的自主接收验证码的能力，以确保长期访问，得鱼不如会渔。

 <img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/9c46ea28ec79e40b4529ccb071138d3.jpg" alt="9c46ea28ec79e40b4529ccb071138d3.jpg|300" style="zoom: 33%;" />



这样的验证流程一般是商家提供我们手机号，我们点击发送验证码，商家再告诉我们他收到的验证码：

 <img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/img_v3_02do_9cde9f43-ddde-4bfa-83bb-3a90665a5f6g.jpg" alt="img_v3_02do_9cde9f43-ddde-4bfa-83bb-3a90665a5f6g.jpg|400" style="zoom: 33%;" />



 ## **Gemini的注册流程**
 准备工作：开启网络工具，使用全局模式。进入Gemini主页：https://gemini.google.com/
 ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912104904.png)
- 如果未成功打开Gemini主页则检查：
  -![|400](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912111647.png)

  1. 先检查是网络工具是否可以正常使用，例如打开油管页面应是正常显示的。
  2. 如果其他网址可以正常显示但Gemini仍然显示如图，则检查节点和网络工具应该为英美地区，不能为亚洲地区，HK也不行。模式应为global全局模式，而不是rule规则模式，direct直连模式。


点击登录，转到 Google 账号登录页面。点击**创建账户**选择个人用途。
   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811191353.png)

2. **填写注册信息**
   - 根据页面指示输入您的姓名、出生日期、性别、设置密码，并确定邮箱地址，直到达到电话号码验证步骤。
   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912105759.png)
   注意年龄要18岁往上，大模型产品部分功能对年龄有限制，即199几年，2000年前
   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912105834.png)
   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919114716.png)

这里就是填写以后你的邮箱地址，所以用户名最好写的便于记忆
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912110020.png)

填写密码了，我们使用的是一次性手机号，如果注册成功后没有自己修改验证手机号码为自己的手机号是找不回来的。所以一定要记住，有时多次输入错误也会被封禁账号。
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912110411.png)
-  小技巧是可以在谷歌注册成功后修改验证手机号为自己的手机号。注意以下步骤是在注册成功后执行的。目的是更改手机号为自己的方便验证和找回密码。
  ![300](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918141836.png)
  ![300](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918141914.png)
  ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918142132.png)

- 接下来就是手机号验证了，国内手机号注册是行不通的。此时就需要借助sms接码平台来绕过地理限制通过购买也用于Gmail服务的不同国家的可用虚拟号20分钟的使用权来收发验证码。
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918140626.png)

- 使用SMS接码平台接收虚拟验证码
	
	1. **注册登入SMS接码平台 SMS-active**
	
	   我们选择的是经过多年验证的老牌主流SMS接码平台——[SMS-Activate](https://sms-activate.io/cn)。进入页面后，点击右上角的注册或登录。可以使用国内邮箱进行注册。为方便教程展示，我们将界面设置为中文。
	
	   ![image.png|277](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811150307.png)
	
	   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240809112950.png)
	
	2. **充值来购买虚拟号码**
	
	   虚拟号码各有不同的价格，此时需进行充值购买。选择支付方式（如支付宝），最低充值金额为2美元。充值完成后，余额可以保留用于后续服务。
	
	   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811140952.png)
	
	   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811145146.png)
	
	3. **激活虚拟号码并等待验证码**
	
	   注册并登录成功后，主界面分为左侧和右侧两个功能区。在左侧搜索框中输入我们需要注册的服务名，需要注册邮箱的用户请搜索Gmail 并展开，选择英格兰或其他热门国家。
		![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811185844.png)
	
		 注意尽量选英美国家，小众国家。重点是排除掉那些战乱或可能同样像国内的一样被限制的国家，如俄罗斯等。如果选的国家没有收到验证码也可以退掉，可以重新试，不会有损失。
		
		 <img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811200928.png" alt="image.png|270" style="zoom: 67%;" />
	
	​	点击右侧的绿色购物车图标，进入购买页面。购买成功后，点击“激活”按钮等待接收验证码。<img src="https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811201438.png" style="zoom: 67%;" />
	
	​	收到验证码后，返回并填入相应字段完成验证。![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811202732.png)
	
	回到谷歌界面填入手机号，并发送验证码。在SMS接码平台上等待接收验证码：
	
	![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811203347.png)

​	回到谷歌界面填入在SMS-active购买虚拟号码，输入接收到的验证码完成验证步骤。

   ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240811203541.png)

添加辅助邮箱可以方便自己找回密码，当然也可以选择跳过

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912110813.png)

恭喜您成功注册谷歌账号！引导我们确认我们的信息，上面是名字，下面是邮箱地址，出现这个的时候就已经成功注册啦！
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912110936.png)
隐私条款，点击同意
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912111325.png)


## 使用Gemini相关产品

### web端Gemini聊天机器人
多个入口:
- 第一种：网址 https://gemini.google.com/
- 第二种：谷歌生态的加持下，可以于谷歌浏览器的地址框上输入@选择Gemini或全拼：@gemini
  输入问题 按enter就跳转到了gemini页面。如果没有此功能，则需升级谷歌浏览器为最新版本。
  ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919114041.png)
  ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919114356.png)
  ![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919114542.png)

不要给精确地地址
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912113534.png)

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919114639.png)
升级了之后可以使用Gem，类似GPTs，Gem 能帮助创建可供 Gemini 重复执行的具体指令。当你与 Gem 对话时，Gemini 将根据你的指令和偏好设置为你量身定制回答。
-  Gem 的用处

	利用 Gem，你可存储针对 Gemini 应用的偏好设置，以节省反复在提示中输入相同目标和准则信息的时间。通过创建一个包含你的所有目标和偏好设置信息的 Gem，或使用为特定操作而设计的预建 Gem，每当你想使用类似的指令探索某个主题时，相应 Gem 就会像快捷方式一样帮你省时省力。
	
	- **锻炼要求。** 创建一个包含任何身体限制和时间限制的 Gem，确保 Gemini 最大限度地利用你的时间，并为每次新锻炼规划合适的运动。
	- **饮食偏好。** 创建一个 Gem，为其提供食谱中应该包含的具体食材或你要遵循的饮食方案（例如素食或高蛋白）；每当你要求它提供新食谱时，它都会遵循这些限制条件。
	- **园艺规范。** 根据花园的气候和光照条件创建一个 Gem，每当你向 Gemini 询问园艺问题时，都能获得相关创意。

## Google AI Studio
[Google AI Studio](https://aistudio.google.com/) 是一个基于浏览器的集成开发环境，用于与生成模型进行原型设计。Google AI Studio 让您快速尝试模型并实验不同的提示。当您构建出满意的作品时，可以将其导出为您喜欢的编程语言的代码，并与 [Gemini API](https://ai.google.dev/gemini-api/docs/quickstart) 一起使用。
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240912115348.png)

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918153411.png)
token count :模型可以接受的文本的最大长度
免费用最新最智能的大模型
 ![400](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919111107.png)

免费微调
![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240919111441.png)
- 调优周期（训练轮数）：
    - 意义：指模型在整个训练数据集上的迭代次数。
    - 设置：从较小的数值（如1-5）开始，根据模型性能建议逐步增加。对于小数据集，可能需要更多轮次，如10-20。小数据集需要更多轮次来充分学习。；大数据集通常能快速收敛，可能很快轮次就足够了。
- 学习率乘数（学习率乘数）：
    - 意义：用于调整预训练模型的基础学习率。1表示保持原有学习率，小于1会降低学习率，大于1会提高学习率。
    - 建议：增大的乘数会导致更大的更新步长，可能会加快学习但也可能导致不稳定。较小的乘数会使更新更稳定，有利于更大的控制但可能会学习得更慢。较小的乘数可以帮助保留更多预训练的知识，而增大的乘数允许模型更快地适应新任务。一般从1开始，如果训练开始可以尝试降低（如0.5或0.1），如果收敛太慢可以尝试稍微提高（如1.5或2）。
- 批次大小 (批量大小):
    - 意义： 梯度模型参数更新处理的样本数量。
    - 设置：根据任务复杂度和可用内存选择，较小的批量（如2或4）确实会引入更多的随机性，中等规模的批量（如4-8）通常被认为能够提供良好的泛化能力，这是因为它在随机性和稳定性之间取得了平衡。增大的批量可以加快训练，但可能需要调整其他参数来保持性能，例如减小批量大小可能需要减小学习率。根据您的GPU内存和数据集大小来选择合适的值。

- 参数调整是一个迭代的过程，需要耐心和实验来找到最佳配置。
### 创建有自己聊天风格的机器人
- 点击 **Create new prompt**

- 点击 **System Instructions** 箭头展开系统提示部分。编写系统提示，创建有鲁迅聊天风格的机器人。
  

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/20241008192211.png)	

- 添加系统说明后，通过与模型聊天开始测试您的应用程序。

- 点击 **Run** 按钮或按 Enter 以获取聊天机器人的响应。

- 一旦对提示原型感到满意，可以使用 **Get code** 按钮开始使用API coding，或保存您的提示以便稍后继续工作并与他人分享。


![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/20241008192328.png)

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/20241008192243.png)

### 微调说话风格展示

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918172058.png)

![image-20241008192615442](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/image-20241008192615442.png)



领取API key
打开[Google AI Studio](https://aistudio.google.com/) ，https://aistudio.google.com/

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918175219.png)

创建APIkey

 ![400](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918175320.png)



![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918175413.png)



如果后续要用可以在箭头处点击展开再次复制

![](https://typora-photo1220.oss-cn-beijing.aliyuncs.com/DataAnalysis/LingYi/20240918175502.png)
