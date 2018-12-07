 ## 产品需求文档

- 发布日期：2018年11月24日 
- 主题：人脸识别+语音签到 
- 文件现状：进行中 
- 文件的主人：张广彬 

### 加值宣言

- >本产品中包含三个人工智能API,分别是百度的人脸对比API、百度的语音识别、API以及高德地图API。其中他们实现的主要功能时签到考勤，但避免了传统考勤系统的毛病（存在虚假考勤的情况）。通过对签到人最直接有效的API智能识别，来使签到考勤的有效性大幅度的提升。当然也会存在不足的地方，但这是进步的基础，如果您发现了不足之处，欢迎联系我，谢谢。

### 核心价值宣言
- >最小可用产品：用最低的成本设计出来只含有核心功能的小程序，核心功能主要围绕着签到功能来进行，通过api来进行不断的核实，最终确定签到人身份
- 为什么使用小程序作为MVP？
- 小程序是一项可选的降低成本的方案，而且小程序是一个强有力支持的大平台，增加最小可用产品实施的可行性。

### 核心价值与用户痛点
- >痛点：课代表点名点错，读错名字，被提早点名，点了答了到但课代表没有听到。等等一系列的问题，都可以通过文中这一与api有关的签到产品来解决。解决了一些列因为人工操作不当所带来的错误，增加课堂签到的有效性。

### AI产品概率性与用户痛点
- >人工智能的产品或服务若迟迟没有得到广泛认可，本质原因是产品从概率上不能满足用户的需求。而对于文中所提过的用户痛点，绝大部分都是可以通过api来解决的，但缺乏相关的测试知识，暂时无法给出具体的人工智能概率数据。所以单从人工所出现的错误来讲，智能api能够解决大部分来自于认为错误的问题。

### 需求列表与人工智能API加值 
- >产品中使用的加值有反映到需求列表中，可用的api有三个，具体的包含如下文所示。

### 产品迭代规划 
- >以用户需求反馈作为迭代根据。在每个月的月底都需要对产品进行总结，发现产品的问题，规划产品未来的发展。

### [交互与界面设计](https://zdnfzgb.github.io/QIMOXIANGMU_FOR_API/)
 - >交互原型：请点击链接查看<https://zdnfzgb.github.io/QIMOXIANGMU_FOR_API/>

### 会用到的API
>百度的人脸对比API、百度的语音识别、API以及高德地图API

### [API的输入与输出](http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/YtKvVLEOck50KcjT7fydOs60mdNhBGbsSb7y9mXIqRs!/b/dDYBAAAAAAAA&bo=wQMuAgAAAAADB8w!&rf=viewer_4)
- 图示：
 ![API的输入与输出](http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/YtKvVLEOck50KcjT7fydOs60mdNhBGbsSb7y9mXIqRs!/b/dDYBAAAAAAAA&bo=wQMuAgAAAAADB8w!&rf=viewer_4
)

### Python代码展示
- 因为mardown中显示ipynb文档的效果不好，请点击链接来查看代码展示，谢谢
> <https://github.com/zdnfzgb/API_ML_AI/blob/master/Python_code_presentation.ipynb>


### [产品工作流程](http://naotu.baidu.com/file/d135db537b7dd495173f374a1c5fb6e4?token=61ed5d774dc91104)
- 流程图：
 ![工作流程图](http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/htVx0hbhStxh8B6otKKwWPzHmLLaxbohUIA2ClMREEQ!/b/dFQBAAAAAAAA&bo=PwfCAQAAAAADB9k!&rf=viewer_4)


### 目标
- 让产品能够有着其存在的价值，或者换句话说能够让想法解决到现实中存在的问题，不枉作者本人的心血，现在正处于完善的阶段，需要不断的支持与大力的建议，谢谢。

### 用户定位
- 学生群体，主要是用于学生的上课签到考勤。

### 背景和战略契合处
- 为什么做这一项产品？主要是因为，平时上课签到很累，而且又浪费时间，又无聊，听着那些名字一个一个念过。而且点名字感觉点和没点都差不多（en。。。你懂得），就想到用API组合起来来签到会更加方便，且大大的减少人力成本。唯一不好的可能是会被不怎么爱上课的同学讨厌？

### 假设
- 用户在使用此产品时，主要是在APP上使用，通过注册登录账号，然后选择自己即将上课的课程。通过GPS定位系统来确定用户是否在上课地点的位置，确定位置之后，方可开始签到。如果GPS功能不可用，需要找到班级对应的老师，让老师进行后台帮助学生签到。
- 需要服务器管理，需要APP的运营者，需要等等......

### 需求
- 用户案例：老师因为点了全班的名字，然后全班推迟了十分钟上课，最后规定的课堂内容讲不完。
- 标题：产品可以改进课堂体验
- 重要程度：一般
- 笔记：无

### 问题
- 可以完成的问题：完成一些基本的签到任务，可以对人脸进行简单的识别，对人声进行简单的识别，最终完成同学的签到。

### 不做
- 暂时不做广告接入，先把产品完善到少bug的状态。 

## 交互与界面设计
- https://zdnfzgb.github.io/QIMOXIANGMU_FOR_API/

## Python代码展示
- https://github.com/zdnfzgb/API_ML_AI/blob/master/Python_code_presentation.ipynb

## API的输入与输出
- http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/YtKvVLEOck50KcjT7fydOs60mdNhBGbsSb7y9mXIqRs!/b/dDYBAAAAAAAA&bo=wQMuAgAAAAADB8w!&rf=viewer_4
 
## 产品工作流程图
- http://naotu.baidu.com/file/d135db537b7dd495173f374a1c5fb6e4?token=61ed5d774dc91104

## 图片：低保真的交互原型
- http://m.qpic.cn/psb?/V11pnbYZ3BKYjZ/dIGegZSSpRLb.H5p.csoTYWwj1rUkdbteNc1KB0t5dQ!/b/dDcBAAAAAAAA&bo=GQRZAgAAAAADF3Q!&rf=viewer_4&t=5
