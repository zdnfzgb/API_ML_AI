## 南苑签到-产品需求文档

- 发布日期：2018年11月24日 
- 主题：人脸识别+语音签到+高德地图定位 
- 文件现状：进行中 
- 文件的主人：张广彬 

**目录**
产品描述|API相关事项|交互原型及其他杂项
---|---|---
[加值宣言](#加值宣言)|[API概率性数据](#概率性数据)|[交互与界面设计](#交互与界面设计)
[核心价值宣言](#核心价值宣言)|[API可用性的方案分析](#可用性的方案分析)|[产品工作流程](#产品工作流程)
[核心价值与用户痛点](#核心价值与用户痛点)|[API的输入与输出](#API的输入与输出)|[产品迭代规划 ](#产品迭代规划 )
[使用场景](#使用场景)|[Python代码展示](#Python代码展示)|[不做](#不做)

### 加值宣言
- 用户定位:学生群体，主要是用于学生的上课签到考勤。
- 本产品是三种API合并来实现主要功能的课堂签到考勤产品，三个API分别是百度的人脸对比API、百度的语音识别、API以及高德地图API。
- 让产品能够有着其存在的价值，或者换句话说能够让想法解决到现实中存在的问题，不枉作者本人的心血，现在正处于完善的阶段，需要不断的支持与大力的建议，谢谢。

### 核心价值宣言
- 最小可用产品：用最低的成本设计出来只含有核心签到功能的小程序，通过三种API来进行用户身份的核实，最终达成精准签到。
	- 为什么使用小程序作为MVP？
	- 小程序是一项可选的降低成本的方案，而且小程序是一个强有力支持的大平台，增加最小可用产品实施的可行性。
	
### 核心价值与用户痛点
- 痛点：课代表点名点错，读错名字，被提早点名，点了答了到但课代表没有听到。等等一系列的问题，都可以通过文中这一与api有关的签到产品来解决。解决了一些列因为人工操作不当所带来的错误，增加课堂签到的有效性。
- 平时上课签到浪费时间，听着名字一个一个念过，也就意味着时间流失。而且实际上的点名效率并不高，存在误签或者代签的情况，该产品刚好可以解决以上问题。

### [产品工作流程](http://naotu.baidu.com/file/d135db537b7dd495173f374a1c5fb6e4?token=61ed5d774dc91104)
- 流程图：
 ![工作流程图](http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/htVx0hbhStxh8B6otKKwWPzHmLLaxbohUIA2ClMREEQ!/b/dFQBAAAAAAAA&bo=PwfCAQAAAAADB9k!&rf=viewer_4)
	
### 使用场景
- 假设
    - 用户在使用此产品时，主要是在APP上使用，通过注册登录账号，然后选择自己即将上课的课程。通过GPS定位系统来确定用户是否在上课地点的位置，确定位置之后，方可开始签到。如果GPS功能不可用，需要找到班级对应的老师，让老师进行后台帮助学生签到。
- 需求
    - 用户案例：老师因为点了全班的名字，然后全班推迟十分钟上课，最后规定的课堂内容讲不完。
    - 标题：产品可以改进课堂体验
    - 重要程度：一般
    - 笔记：无
- 问题
    - 可以完成的问题：完成一些基本的签到任务，可以对人脸进行简单的识别，对人声进行简单的识别，最终完成同学的签到
- 需求列表与人工智能加值 
	- 产品中使用的加值有反映到需求列表中，可用的api有三个，具体的包含如下文所示。

### [交互与界面设计](https://zdnfzgb.github.io/QIMOXIANGMU_FOR_API/)
- 交互原型：请点击链接查看<https://zdnfzgb.github.io/QIMOXIANGMU_FOR_API/>

### 概率性数据
- 人工智能的产品或服务若迟迟没有得到广泛认可，本质原因是产品从概率上不能满足用户的需求。而对于文中所提过的用户痛点，绝大部分都是可以通过api来解决的，但缺乏相关的测试知识，暂时无法给出具体的人工智能概率数据。所以单从人工所出现的错误来讲，智能api能够解决大部分来自于认为错误的问题。

### 可用性的方案分析

- 拟定方案：现在产品先满足的是初期的使用，QPS数量为10基本可以满足产品的测试，如果测试完成，可根据实际的用户数量来决定具体的购买量。根据下表的定价算出这样的价格方案。
	- 百度人脸识别API价格（按月购买）：10×300=3000
	- 高德地图API价格：0
	- 百度语音识别API价格：0
	- 总价格：QPS数量为10的情况下，每月仅需支付3000元。

**1. 百度人脸对比API定价表**

购买的QPS数量 | 按月购买 | 按天购买      
---|---|---
0< QPS <=10 | 300元/月/QPS | 30元/天/QPS
10< QPS <=50 | 250元/月/QPS | 25元/天/QPS
50< QPS <=100 | 200元/月/QPS | 20元/天/QPS
100< QPS  | 150元/月/QPS | 15元/天/QPS
> 说明：QPS（query per second）指每秒向服务发送的请求数量峰值，相当于每个API每秒可以允许请求的最大上限数量。

**2. 高德地图API定价表**

<table border=0 cellpadding=0 cellspacing=0 width=518 style='border-collapse:
 collapse;table-layout:fixed;width:388pt'>
 <col class=xl65 width=72 style='width:54pt'>
 <col class=xl65 width=116 style='mso-width-source:userset;mso-width-alt:3712;
 width:87pt'>
 <col class=xl65 width=104 style='mso-width-source:userset;mso-width-alt:3328;
 width:78pt'>
 <col class=xl65 width=131 style='mso-width-source:userset;mso-width-alt:4192;
 width:98pt'>
 <col class=xl65 width=95 style='mso-width-source:userset;mso-width-alt:3040;
 width:71pt'>
 <tr height=18 style='height:13.5pt'>
  <td rowspan=2 height=54 class=xl66 width=72 style='height:40.5pt;width:54pt'>服务</td>
  <td colspan=2 class=xl66 width=220 style='border-left:none;width:165pt'>个人开发者</td>
  <td colspan=2 class=xl66 width=226 style='border-left:none;width:169pt'>企业开发者</td>
 </tr>
 <tr height=36 style='height:27.0pt'>
  <td height=36 class=xl67 width=116 style='height:27.0pt;border-top:none;
  border-left:none;width:87pt'>日调用超量封停（次/日）</td>
  <td class=xl67 width=104 style='border-top:none;border-left:none;width:78pt'>QPS<br>
    （次/秒）</td>
  <td class=xl67 width=131 style='border-top:none;border-left:none;width:98pt'>日调用超量封停<br>
    （次/日）</td>
  <td class=xl67 width=95 style='border-top:none;border-left:none;width:71pt'>QPS<br>
    （次/秒）</td>
 </tr>
 <tr height=26 style='mso-height-source:userset;height:19.5pt'>
  <td height=26 class=xl66 style='height:19.5pt;border-top:none'>地理编码</td>
  <td class=xl66 style='border-top:none;border-left:none'>6000</td>
  <td class=xl66 style='border-top:none;border-left:none'>100</td>
  <td class=xl66 style='border-top:none;border-left:none'>3000000</td>
  <td class=xl66 style='border-top:none;border-left:none'>1000</td>
 </tr>
</table>

**3. 百度语音识别API定价规则**

- 百度官方问答
    - Q：语音识别、合成接口每天调用限额是多少，如何申请提高限额？
    - A：语音识别、合成接口调用量无限。QPS识别默认为10，合成为100，申请提高配额，请登录控制台，点击百度语音，选择应用列表，选择对应应用，查看详情，点击申请提高配额，一般会在2个工作日内完成审核。


### [输入与输出](http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/YtKvVLEOck50KcjT7fydOs60mdNhBGbsSb7y9mXIqRs!/b/dDYBAAAAAAAA&bo=wQMuAgAAAAADB8w!&rf=viewer_4)
- 图示：
 ![API的输入与输出](http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/YtKvVLEOck50KcjT7fydOs60mdNhBGbsSb7y9mXIqRs!/b/dDYBAAAAAAAA&bo=wQMuAgAAAAADB8w!&rf=viewer_4
)

### 代码展示
- 因为mardown中显示ipynb文档的效果不好，请点击链接来查看代码展示，谢谢
	- 代码链接：<https://github.com/zdnfzgb/API_ML_AI/blob/master/Python_code_presentation.ipynb>
	- [备用链接](http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/twiQlMDz0fEg7Huc40r6oHBgFleql7NC9xTaavTfMus!/b/dL8AAAAAAAAA&bo=1ANiB9QDYgcDCSw!&rf=viewer_4)：如果github长时间加载不出来代码页面，请点击备用链接。

### 不做
- 暂时不做广告接入，先把产品完善到少bug的状态。 

### 产品迭代规划 
- 2018-12-10：添加展示原型
- 2018-12-14：完善代码展示
- 2018-12-25：补充API的产品定价表
- 2018-12-26：在原型展示中补充引导

 *** 

## 清单
- Python代码展示 <https://github.com/zdnfzgb/API_ML_AI/blob/master/Python_code_presentation.ipynb>

- 【备用】代码展示截图图片：<http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/twiQlMDz0fEg7Huc40r6oHBgFleql7NC9xTaavTfMus!/b/dL8AAAAAAAAA&bo=1ANiB9QDYgcDCSw!&rf=viewer_4>

- API的输入与输出:<http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/YtKvVLEOck50KcjT7fydOs60mdNhBGbsSb7y9mXIqRs!/b/dDYBAAAAAAAA&bo=wQMuAgAAAAADB8w!&rf=viewer_4>


- 产品工作流程图 :<http://naotu.baidu.com/file/d135db537b7dd495173f374a1c5fb6e4?token=61ed5d774dc91104>


- 交互原型 ：<http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/dIGegZSSpRLb.H5p.csoTYWwj1rUkdbteNc1KB0t5dQ!/b/dDcBAAAAAAAA&bo=GQRZAgAAAAADF3Q!&rf=viewer_4&t=5>