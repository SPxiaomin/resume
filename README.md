# 谷俊民个人简历

微信: SPxiaomin-boy

邮箱: gujunmin84@gmai.com

github: https://github.com/SPxiaomin

## 自我介绍

本人目前已经工作经验三年+「饿了么 + 字节」，

热爱技术，热爱生活，

擅长解决问题，

是一个自我驱动型的人，

主要技术栈——全栈JS.

## 业余项目

高可配置脚手架 https://github.com/SPxiaomin/highly-configurable-cli

## 项目经验

### 图片编辑「1年+」

背景&目标
* 目前，字节主要的商业模式是多边商业模式——通过补贴创作者创造有趣、有价值的信息吸引流量，然后通过广告变现. 因为降低成本对公司来说是很重要的.
* 在公司内部，按照之前的模式，每新建一个广告，至少需要一个设计师来设计相应的广告投放图片. 随着越来越多地广告被创建，需要更多设计师. 除此之外，设计师的成本不是线性的，因为需要有管理成本和沟通成本.
* 
* 因此就产生了这个项目. 项目有两个产品线. 一是图片效果增强，就是在广告主提供了投放图片的情况下，为其添加特效，辅助其提高转化率. 另一个是AI图片，广告主可以根据选项进行相应的输入，然后会产出多张图片给广告主，广告主后续可以在编辑生态工具进行编辑.

角色&责任  
* 负责图片编辑工具生态的建设.
* 
* 支持更多的业务线.
* 完善编辑生态.

项目挑战  
* Iframe 简化编辑器
  * 各种系统需要图片编辑画板，但是不需要其他的复杂编辑模块. 以及想把其集成到自己的系统中去. 因为我将图片编辑画板进行了拆分，成为一个独立的组件复用，然后以iframe形式进行导出. 其他系统通过iframe api进行沟通.
* 
* 可配置编辑能力
  * 对于线上图片编辑系统，需要支持较多的业务线进行图片编辑. 因此如果代码未进行良好设计，会是一团糟. 总体来说，系统主要两块，一是编辑器，二是业务. 不同业务需要不同编辑功能. 于是通过将编辑器单独抽离一层，然后通过参数进行控制.
* 
* 图片渲染
  * 这是线上编辑生态的核心部分. 一般来说，总共4个渲染方法，svg to image/canvas to image/puppeteer/render engine like webkit. 我初步选择了puppeteer方案，因为是个后端方案，可以在多个系统被使用到，并且具备较好地可扩展性. 但是这个方法是低性能地，4台 4g/8core的服务器，qps才40. 因此，与此同时在尝试将webkit中渲染部分抽离，但是由于业务调整，项目被交到其他项目去了.

### 广告联盟转化卡「0.5年+」

背景&目标
* 公司存在一定量的第三方流量，因此公司通过了一个sdk的方式帮助第三方流量进行变现，项目的目的是提供一个平台用于管理和编辑广告样式.
* 
* 项目存在两个系统，一个是管理样式，一个是用于编辑样式以及webview h5渲染.

角色&责任
* 参与编辑部分开发，提供广告需要的编辑组件.
* 负责h5渲染的UI自动化探索. 这部分存在的原因是QA开发的资源不够，以及每次h5渲染引擎改变的时候都要手动进行线上样式渲染检测，非常耗费不必要人力资源. 后期采用了appium + node.js报告服务的方式进行了解决，但是后续QA开发资源恢复，因此将项目交回了QA侧.

项目挑战  
* 项目最具挑战性地就是UI自动化从0到1的探索，因为在这之前，我没有任何经验. 解决问题最关键地就是耐心，不断搜索/学习/实验.

### 编辑中台「4月+，初期是上海和北京合作开发，后期由于团队调整，交予北京」

背景&目标
* 项目中存在非常多业务相关的项目，每次都要重复进行编辑能力地开发，因此非常必要进行编辑部分的复用抽离.
* 
* 技术方案: 编辑器的每一部分都是组件，可以进行任意业务需求组合. 通过一个core.js进行通信「tapable.js」. 每一个组件可以通过配置进行扩展.

角色&责任
* 项目整体的架构设计.
* 业务支持.

项目挑战
* 项目更多是编辑开发经验的抽象，不具备太大挑战.

## 最后

感谢您花费宝贵的时间阅读完我的简历，期待和您共事.

# Junmin Gu's Resume

wechat: SPxiaomin-boy

email: gujunmin84@gmai.com

github: https://github.com/SPxiaomin

## Self Intro

My name's Junmin Gu.

I have worked for over three years「eleme + bytedance」.

I'm good at problem solving and quite self-motivated.

My main tech stack is JS full stack.


## Spare-Time Projects

highly-configurable cli https://github.com/SPxiaomin/highly-configurable-cli

## Project-Related Experience

### image editor.「over one year」

situation & target:
* Currently, the main business mode of bytedance is a multisided business mode. It subsidizes the platform authors to create interesting and valuable information to attract more traffic, and then earns money through the advertisements. So reducing the cost of the company is an important part.
* In company, when creating a new advertisement, at least one designer is needed to design images as required. As more and more advertisements are created, more designers are needed. Besides, the cost of designer payment is not linear, as you need to hire some managers and there are cooperation cost.
* 
* So, we decided to reduce the un-linear design cost. There were two product lines. One was image enhancement. That meant adding special effects on existing images provided by the advertisers, in order to help them to increase conversion rate. The other was AI picture, where people can get mutiple images by inputing the opinionated attributes and then edit them through the online tools.

my role and reponsibilities: 
* I was leading the online image-related tool ecosystem.
*   
* supporting more and more business lines.
* perfecting the tool ecosystem. 
    * 「done」online editor.
    * 「done」template system.
    * image cropping tool.
    * vertical advertising industy image gallery. (cooperating with 图虫.

project challenges:
* iframe.
    * various systems needed to get the core image edit function「the canvas」, rather than all the detailed edit functions. And they wanted to integrate it into their systems. So I extracted the core image edit function as a seperate component and exported an iframe. Other systems communicated with it through the iframe api.
* 
* configurable editor functions.
    * As for the online image editor system, it had to support many business lines to edit images. So, if the code had not been designed well, the code would have been in a mess. In the grand scheme of things, there were two parts. One was editor, the other was business. Different businesses needed different editor functions. So, I extracted the editor as a separate layer and made its functions configurable by the different parameters.
* 
* image render.
    * This was the core part of online tool ecosystem. Generally speaking, there were four methods to produce images, svg to image / canvas to image / puppeteer / render engine like webkit. I used the puppeteer method, because it’s a backend method which could be used in multiple frontend systems and had more extendibility. But this method was low-performant, which could only support 40qps by 3 4g/8core servers. So I tried to create a render engine, the general idea was to extract only the related parts from webkit to reduce unnecessary overheads, but meanwhile, due to the business adjustment, the project was transferred to another team.
### ad union conversion cards.「almost half a year」

situation & target: 
* There was some third-party traffic in company. we provided a SDK for third-party apps to show our advertisements. The project aimed to provide a platform for managing and editing the advertisement styles.
*  
* There were two systems, one for managing the styles, and the other for editing the styles and h5 style render in webview.

my role and responsibilities:
* I was involved in the editor part, supporting the style components that the advertisements wanted to get.
* And I was leading the UI automation of the regression testing for h5 style render. The reason for this part was due to the lack of QA-developers and the duplication of checking online style render every time the h5 style render engine was upgraded. But after the offline scheme「appium + nodejs server for reports」 was carried out, this part was transferred to QA team, because then they hired several QA-developers and the project was more appropriate to be in QA team.

project challenges:
* The most challenging part for me in this project was the process from 0 to 1 for UI automation. Because before that I hadn’t have any experience. The key solution was patience for searching, learning and experimenting.

### editor middleground.「4 months, the project was worked on together in shanghai and beijing, due to the team positioning, it was transferred to beijing」

situation & target: 
* There were many editor related businesses in the team. The team members needed to develop the similar editor features. So It was very necessary to extract the editor layer as a seperate part to be reused.
* 
* Tech scheme: Every part of the editor was a component and you could combine them as you wished. And there was a core.js for communicating「tapable.js」. Every component could be extended by configurations.

my role and responsibilities:
* I was involved in the architecture design work and the render component.
* supporting business lines.

project challenges:
* no impressive challenges.

## In the End

Thank you for taking the time to read my resume. Look forward to working with you.
