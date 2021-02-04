# Junmin Gu's Resume

phone: 

education：Hunan University of Science and Technology, Computer Science Information Security, 2018-6 graduated

wechat: SPxiaomin-boy

email: gujunmin84@gmail.com

github: https://github.com/SPxiaomin

## Self Intro

My name's Junmin Gu.

I have worked for over three years。

2017/12-2019/4, eleme.

2019/4-now, bytedance.

I'm good at problem solving and quite self-motivated.

My main tech stack is JS full stack.


## Spare-Time Projects

highly-configurable cli https://github.com/SPxiaomin/highly-configurable-cli

## Project-Related Experience

### image editor.「over one year」

situation & target:  

- Currently, the main business mode of bytedance is a multisided business mode. It subsidizes the platform authors to create interesting and valuable information to attract more traffic, and then earns money through the advertisements. So reducing the cost of the company is an important part.  
- In company, when creating a new advertisement, at least one designer is needed to design images as required. As more and more advertisements are created, more designers are needed. Besides, the cost of designer payment is not linear, as you need to hire some managers and there are cooperation cost.  
- So, we decided to reduce the un-linear design cost. There were two product lines. One was image enhancement. That meant adding special effects on existing images provided by the advertisers, in order to help them to increase conversion rate. The other was AI picture, where people can get mutiple images by inputing the opinionated attributes and then edit them through the online tools.

my role and reponsibilities:   

- I was leading the online image-related tool ecosystem.  
- supporting more and more business lines.  
- perfecting the tool ecosystem.  
    - 「done」online editor.  
    - 「done」template system.  
    - image cropping tool.  
    - vertical advertising industy image gallery. (cooperating with 图虫.  

project challenges:  

- iframe.  
    - various systems needed to get the core image edit function「the canvas」, rather than all the detailed edit functions. And they wanted to integrate it into their systems. So I extracted the core image edit function as a seperate component and exported an iframe. Other systems communicated with it through the iframe api.

- configurable editor functions.  
    - As for the online image editor system, it had to support many business lines to edit images. So, if the code had not been designed well, the code would have been in a mess. In the grand scheme of things, there were two parts. One was editor, the other was business. Different businesses needed different editor functions. So, I extracted the editor as a separate layer and made its functions configurable by the different parameters.

- image render.  
    - This was the core part of online tool ecosystem. Generally speaking, there were four methods to produce images, svg to image / canvas to image / puppeteer / render engine like webkit. I used the puppeteer method, because it’s a backend method which could be used in multiple frontend systems and had more extendibility. But this method was low-performant, which could only support 40qps by 3 4g/8core servers. So I tried to create a render engine, the general idea was to extract only the related parts from webkit to reduce unnecessary overheads, but meanwhile, due to the business adjustment, the project was transferred to another team.

### ad union conversion cards.「almost half a year」

situation & target:  

- There was some third-party traffic in company. we provided a SDK for third-party apps to show our advertisements. The project aimed to provide a platform for managing and editing the advertisement styles.  
- There were two systems, one for managing the styles, and the other for editing the styles and h5 style render in webview.

my role and responsibilities:  

- I was involved in the editor part, supporting the style components that the advertisements wanted to get.  
- And I was leading the UI automation of the regression testing for h5 style render. The reason for this part was due to the lack of QA-developers and the duplication of checking online style render every time the h5 style render engine was upgraded. But after the offline scheme「appium + nodejs server for reports」 was carried out, this part was transferred to QA team, because then they hired several QA-developers and the project was more appropriate to be in QA team.

project challenges:  

- The most challenging part for me in this project was the process from 0 to 1 for UI automation. Because before that I hadn’t have any experience. The key solution was patience for searching, learning and experimenting.

### editor middleground.「4 months, the project was worked on together in shanghai and beijing, due to the team positioning, it was transferred to beijing」

situation & target:  

- There were many editor related businesses in the team. The team members needed to develop the similar editor features. So It was very necessary to extract the editor layer as a seperate part to be reused.  
- Tech scheme: Every part of the editor was a component and you could combine them as you wished. And there was a core.js for communicating「tapable.js」. Every component could be extended by configurations.

my role and responsibilities:  

- I was involved in the architecture design work and the render component.  
- supporting business lines.

project challenges:  

- no impressive challenges.

## In the End

Thank you for taking the time to read my resume. Look forward to working with you.
