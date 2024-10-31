---
layout: center
highlighter: shiki
css: unocss
colorSchema: dark
transition: fade-out
mdc: true
glowSeed: 4
title: 交互设计开发规范分享
---

![](/xmd-logo-animated.svg){.w-30.mt--10.mb-5}

<!--
大家好，非常开心能来到这里，今天会议的内容主要是想和大家分享一些交互设计方面的知识和常见的规范。
-->

---
layout: intro
class: pl-40
glowSeed: 14
---

# 设计基础知识分享 &&emsp;&emsp;&emsp; 交互规范分享{.font-serif}

<div class="leading-10 opacity-80">
2024-11-01<br>
大前端研发组<br>
圈圈⭕️<br>
</div>

<div my-10 w-min flex="~ gap-1" items-center justify-center>
  <div i-ri-user-3-line op50 ma text-xl />
  <div><a href="https://vidorra.life" target="_blank" class="border-none! font-300">vidorra.life</a></div>
  <div i-ri-github-line op50 ma text-xl ml4/>
  <div><a href="https://github.com/ROYIANS" target="_blank" class="border-none! font-300">ROYIANS</a></div>
</div>

<img src="https://www.vidorra.life/_next/image?url=https%3A%2F%2Fvidorra.life%2Fapi%2Fv2%2Fobjects%2Favatar%2Fzow48gbjloxg40qz8g.png&w=384&q=75" v-click absolute bottom-30 right-40 h-35 rounded-full />
<img src="/hi.png" v-after absolute top-67 right-80 w-8 rotate-10 delay-300 />

<div flex="~ gap2">

</div>

<!--
首先我来介绍一下我自己，我是圈圈，from 小梦岛。

[click] 然后，我的个人主页和 GitHub 主页，大家可以通过下面的链接访问。
-->

---
layout: cover
title: 产品设计中的质量保证和落地
---

<h1 flex="~ col">
<div text-2xl font-serif origin-top-left transition duration-500 :class="$clicks <= 2 ? 'scale-150' : 'op50'">
  <span v-click>优秀的 </span>
  <span>产品设计 </span>
  <sup text-xs v-click>交互/视觉/整体体验</sup>
</div>
<div mt1 forward:delay-300 font-serif v-click>交互设计之道</div>
</h1>

<div abs-br mx-10 my-11 flex="~ col gap-4 items-end" text-left v-click="1">
  <span>ROYIANS</span>
  <div text-xs opacity-75 mt--4>Nov. 1st 2024</div>
  <!-- <img src="/frontend-nation.svg" w-35 /> -->
</div>

<!--
我们先从一个基本概念说起——产品设计。[click]

在产品开发中，优秀的产品设计至关重要。它不仅帮助我们解决用户的问题，还能确保我们的产品具有高度的可用性和吸引力。[click]

具体来说，优秀的产品设计涵盖了多个方面，包括交互设计、视觉设计以及整体用户体验。它们各自有着不同的关注点和职责。

视觉设计主要关注产品的视觉呈现和美感，
通过色彩、排版、样式等视觉元素来打造产品的外观和风格。

而用户体验设计是一种思想和方法论，它关注整体的用户感受和体验，包括行为、认知、情感等多个方面。
通过从用户需求出发，研究用户的行为习惯、心理特征和需求痛点，以设计出符合用户期望和需求的产品。


而交互设计是我们今天的重点，交互设计主要关注用户与产品之间的互动过程，包括操作逻辑、界面布局、交互方式等。通过合理的设计，
让产品在使用过程中更加顺畅、自然，提供良好的操作体验。交互是连接用户需求与产品功能的重要桥梁。[click]


所以今天的主题就是交互设计之道路。
-->

---
glowX: 100
glowY: 80
---

### How to understand Interaction Design Spec {.op50.mb-2}

<div>
<h1 font-serif>如何「理解」交互设计</h1>
<img src="/r-gui-fan.png" rounded-lg w-120 border="~ gray/50" mt-10 absolute left-70 top-50 v-click="2" />
</div>

<div mt-10 text-xl  font-serif  v-click="1">

一个成熟的设计规范对 产品设计、研发开发、用户使用 都有着重要的指导作用

</div>

<!--
说起设计规范，其实大家都不陌生，一个成熟的设计规范对 产品设计、研发开发、用户使用 都有着重要的指导作用。

产品设计：保障产品内不同模块的设计一致性，同时提高不同设计师间的设计、协作效率

研发开发：通过定义的标准规范，提高流程、组件的复用率，提高整体开发效率

用户使用：让用户能够在产品全局感受到统一且完整的体验，降低使用成本和学习难度

而一个完整的设计规范一般分成「视觉」「交互」两个部分合并组成，在全局原则的指导下，侧重不同的维度和内容分别展开规范的定义，最后再合到一起形成一份完整的设计规范。
-->

---
layout: center
class: text-center
glowX: 50
glowY: 100
---

<h1 important-text-5xl font-serif v-click>什么是「用户体验要素」?</h1>

<div text-white:50 text-2xl font-hand v-click>
从 5 个要素 <span text-yellow2 italic v-mark.yellow.underline.delay300="2">自下而上</span> 的建设 <span text-lime2 v-mark.lime.underline.delay700="2">用户体验</span>
</div>

<!--
在讲交互规范之前，我们先来了解一些名词，因为了解用户界面（UI）的设计原理、用户体验和用户友好设计，

对于我们开发工程师来讲，是一个战略优势。我们只有先了解这些内容，才能更好的理解系统如何开发，在我们的开发中预测出潜在的问题，并确保可以避免一些常见的用户不友好的问题。

然后我们就可以首先是提效，其次是避免债务和重新设计，以及与我们设计团队之间的摩擦。

而我们一旦掌握这个优势，我们的产品开发团队，就可以更快更好地交付高质量的产品，并以更低成本减少错误。[click]

那么，我们先来聊聊用户体验要素。

什么是用户体验要素呢？用户体验是用户在使用产品过程中的主观感受，不仅仅是用户对于产品的功能感受，

还包括产品页面、内容、颜色、字体、逻辑、流程、交互等多个方面。优秀的产品设计团队，能够在产品设计的过程中有意识地系统性优化用户体验。

[click]每个层面的选择，都会受到其上一层面的决策的约束，其核心在于产品底层逻辑根本决定上层形态构成。
-->

---
glow: right
class: text-center
clicks: 5
title: 战略、范围、结构、框架、表现
---

<div transition duration-800 :class="$clicks < 2 ? 'translate-y-45' : ''" relative>

# 战略、范围、<span v-mark.green.underline="1">结构、 框架</span><span absolute right-31.2 v-mark.yellow.underline.delay800="1">框架、表现</span>

<div font-hand bold absolute rotate--4 left-150 top-13 text-3xl text-yellow delay-300 v-click="1">视觉规范</div>
<div font-hand bold absolute rotate--2 left-120 top-12 text-3xl text-green delay-200 v-click="1">交互规范</div>

</div>

<div left-45 top-15 relative transition duration-400 forward:delay-600 v-click="2">
  <img src="/r-yong-hu-tiyan-yao-su.png" w-120 absolute left-0 top-0 rounded />
</div>
<a text-xl pb-10 absolute left-10 v-click="3" href="https://www.uisdc.com/experience-design-elements" target="_blank">→了解更多←</a>

<div absolute left-10 top-45 delay-200 v-click="4">
    <div font-hand bold text-yellow text-3xl pb-10>视觉规范</div>
    <ul>
        <li>图形元素</li>
        <li>色彩体系</li>
        <li>字体体系</li>
        <li>界面布局</li>
        <li>质感风格</li>
        <li>动画动效</li>
    </ul>
</div>

<div absolute right-15 top-45 delay-200 v-click="5">
    <div font-hand bold text-green text-3xl pb-10>交互规范</div>
    <ul>
        <li>全局原则</li>
        <li>页面布局</li>
        <li>通用流程</li>
        <li>标准组件</li>
        <li>文案规范</li>
    </ul>
</div>

<!--
我们先看下是哪五个要素

[click][click]视觉主要是在「表现层」「框架层」进行规范的统一，而交互则是在「结构层」「框架层」进行规范的统一。

[click]就是这五层，大家下来可以访问这篇文章深入的理解一下。
-->

---
glow: right
class: text-center
---

# 视觉角度

<div text-left>从用户体验要素来看，视觉主要是在「表现层」「框架层」进行规范的统一</div>
<div text-left>主要包括：形、色、字、构、质、动 六个层面。</div>

<div left-60 top-5 relative transition duration-400 forward:delay-600 v-click>
  <img src="/r-shi-jue-jiao-du.png" w-100 absolute left-0 top-0 rounded />
</div>

<!--
从用户体验要素来看，视觉主要是在「表现层」「框架层」进行规范的统一，主要包括：形、色、字、构、质、动 六个层面。
-->

---
glow: right
class: text-center
---

# 交互角度

<div text-left>交互角度相对抽象，主要针对于产品的「结构层」「框架层」入手，定义统一的交互规范，指导页面、流程搭建和组件使用规则。</div>
<div text-left>包括：全局原则、页面布局、通用流程、标准组件、文案规范。</div>

<div left-60 top-5 relative transition duration-400 forward:delay-600 v-click>
  <img src="/r-jiao-hu-jiao-du.png" w-100 absolute left-0 top-0 rounded />
</div>

<!--
而交互角度相对抽象，主要针对于产品的「结构层」「框架层」入手，定义统一的交互规范，指导页面、流程搭建和组件使用规则。包括：全局原则、页面布局、通用流程、标准组件、文案规范。

整体维度呈“从抽象到具体的总分关系”，不仅对产品的各个维度都有具体的交互指导，而且不仅能保证长期使用，避免重复返工；同时也便于囊括后续的迭代内容。而这些内容，就是我们通常定义的交互规范，也是交互参与定义设计规范的发力点。

这就是对交互规范的一个基本的认识
-->

---
glowX: 100
glowY: 80
---

### The Right Time to Establish Design Guidelines {.op50.mb-2}

<div>
<h1 font-serif>建立设计规范的时机</h1>
<img src="/h-jianli-sheji-guifan-shiji.png" rounded-lg w-170 border="~ gray/50" mt-10 absolute left-10 top-30 v-click="3" />
</div>

<div mt-10 text-xl  font-serif  v-click="1">
产品探索初期：

搭建范围：「全局说明」「页面布局」「通用流程」
</div>

<div mt-10 text-xl  font-serif  v-click="2">
产品稳定发展期：

搭建范围：「全局说明」「页面布局」「通用流程」「基础组件」「业务组件」
</div>

<!--
产品有不同发展阶段，设计规范同样也有，不同阶段下的产品目标和规范需要覆盖的内容都不尽相同。我们要既要避免做多，保证投入产出比最大化；同时也要构建一个合理的规范迭代思路。 
 
产品探索初期： 
该阶段的产品核心目标是「验证产品或商业模型」，业务需求都是小步快跑、频繁迭代。产品处于从0到1的野蛮生长状态，存在着“先满足功能，再优化体验”的情况，导致该阶段的产品体验往往不太过关。 
 
搭建目的：通过定义原则，梳理关键页面和流程，搭建基本的规范框架。既让团队对产品有统一的设计价值观和认知判断；从页面到流程，又能对应设计参照标准；同时业务可以在规定的框架下发展，不仅让产品体验的根基牢固，而且不会限制功能设计自由。 
 
搭建范围：「全局说明」「页面布局」「通用流程」 
 
产品稳定发展期： 
该阶段的产品基本形态已稳定，也形成了初步的模型结构。后续迭代是在现有结构的基础上，进行增加或优化功能。虽然探索期定义了产品原则、布局和流程，但探索期产品的自由生长，会导致不少设计细节不一致，从而影响了产品整体的体验和效率。 
 
搭建目的：通过回溯整理过往设计，沉淀优化成完整的交互规范。再根据规范统一产品体验，进一步优化流程和效率， 让整个产品体验达到相对稳定的状态。 
 
搭建范围：「全局说明」「页面布局」「通用流程」「基础组件」「业务组件」

-->

---
glowX: 100
glowY: 80
---

### Nielsen's Ten Usability Heuristics {.op50.mb-2}

<div>
<h1 font-serif>尼尔森的十大可用性原则</h1>
<img src="/h-nikesen-shi-rule.png" rounded-lg w-170 border="~ gray/50" mt-10 absolute left-10 top-30 v-click="1" />
</div>

<!--
尼尔森的十大可用性原则是尼尔森博士在分析了两百多个可用性问题的基础上，提炼出的十项交互设计原则。被广泛运用于网页、APP以及各种人机交互领域。 
 
要注意的是，这10项原则是启发式（heuristics）的、广泛的经验法则，可以指导我们更具价值的思考界面设计。 
 
设计原则都可灵活运用于各个地方,可以是交互设计,也可以是界面设计,深入了解各种设计原则,让设计师在做设计的时候可以找到更好的解决方案,提高用户的使用体验。
-->

---
glowX: 100
glowY: 80
---

<div>
<h1 font-serif>常见交互规范 && 推荐阅读</h1>
</div>

- https://www.zcool.com.cn/work/ZNTA0ODM4ODg=.html
- https://www.zcool.com.cn/work/ZNTA0ODM4MTY=.html

- https://tdesign.tencent.com/design/values
- https://ant-design.antgroup.com/docs/spec/introduce-cn

- https://www.uisdc.com/enhance-the-user-experience-model


---
layout: intro
class: text-center pb-5
glowX: 50
glowY: 120
---

# Thank You!

Slides can be found on [vidorra.life](https://vidorra.life/talks)

<!--
That's all for my talk, thank you, and happy hacking!
-->
