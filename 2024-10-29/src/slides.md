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
大家好，非常开心能来到这里，今天我要分享的内容是关于交互设计开发规范的。
-->

---
layout: intro
class: pl-40
glowSeed: 14
---

# 交互设计开发规范分享

<div class="leading-10 opacity-80">
2024-10-28<br>
大前端研发组<br>
圈圈⭕️<br>
</div>

<div my-10 w-min flex="~ gap-1" items-center justify-center>
  <div i-ri-user-3-line op50 ma text-xl />
  <div><a href="https://vidorra.life" target="_blank" class="border-none! font-300">vidorra.life</a></div>
  <div i-ri-github-line op50 ma text-xl ml4/>
  <div><a href="https://github.com/ROYIANS" target="_blank" class="border-none! font-300">ROYIANS</a></div>
</div>

<img src="/royians-hi.png" v-click absolute bottom-0 right-0 h-86 />
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
<div text-2xl origin-top-left transition duration-500 :class="$clicks <= 2 ? 'scale-150' : 'op50'">
  <span v-click>产品开发中的 </span>
  <span>设计模式 </span>
  <sup text-xs v-click>交互/视觉/整体体验</sup>
</div>
<div mt1 forward:delay-300 v-click>交互规范分享</div>
</h1>

<div abs-br mx-10 my-11 flex="~ col gap-4 items-end" text-left v-click="1">
  <span>ROYIANS</span>
  <div text-xs opacity-75 mt--4>Nov. 1st 2024</div>
  <!-- <img src="/frontend-nation.svg" w-35 /> -->
</div>

<!--
这里是讲演文本，TODO
-->

---
glowX: 100
glowY: 80
---

### How to understand Interaction Design Spec {.op50.mb-2}

<div>
<h1>如何「理解」交互规范</h1>
<img src="/r-gui-fan.png" rounded-lg w-120 border="~ gray/50" mt-10 absolute left-70 top-50 v-click="2" />
</div>

<div mt-10 text-xl  v-click="1">

一个成熟的设计规范对 产品设计、研发开发、用户使用 都有着重要的指导作用

</div>

<!--
The previous episode was about the "Set Theory", where I have already given in a few conferences.

The topic was independent from today's, so no worries if you missed it.

[click] And in case you are interested, you can find the recordings on my website antfu.me afterwards.
-->

---
layout: center
class: text-center
glowX: 50
glowY: 100
---

<h1 important-text-5xl v-click>什么是「用户体验要素」?</h1>

<div text-white:50 text-2xl v-click>
从 5 个要素 <span text-yellow2 italic v-mark.yellow.underline.delay300="2">自下而上</span> 的建设 <span text-lime2 v-mark.lime.underline.delay700="2">用户体验</span>
</div>

<!--
So first
-->

---
glow: right
class: text-center
clicks: 5
title: 战略、范围、结构、框架、表现
---

<div transition duration-800 :class="$clicks < 3 ? 'translate-y-45' : ''" relative>

# 战略、范围、<span v-mark.green.underline="2">结构、 框架</span><span absolute right-31.2 v-mark.yellow.underline.delay800="2">框架、表现</span>

<div font-hand bold absolute rotate--4 left-150 top-13 text-3xl text-yellow delay-300 v-click="2">视觉规范</div>
<div font-hand bold absolute rotate--2 left-120 top-12 text-3xl text-green delay-200 v-click="1">交互规范</div>

</div>

<div left-45 top-15 relative transition duration-400 forward:delay-600 v-click="3">
  <img src="/r-yong-hu-tiyan-yao-su.png" w-120 absolute left-0 top-0 rounded />
</div>

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
So assume
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
So assume
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
整体维度呈“从抽象到具体的总分关系”，不仅对产品的各个维度都有具体的交互指导，而且不仅能保证长期使用，避免重复返工；同时也便于囊括后续的迭代内容。而这些内容，就是我们通常定义的交互规范，也是交互参与定义设计规范的发力点。
-->

---
class: text-2xl
glow: right
title: Make things easier!
---

# Make things <span font-hand text-green scale-110 ml1 inline-block>Easier!</span>

<div flex="~ gap-2 items-center" text-indigo mt-15 v-click>
  <div i-ph-hammer-duotone text-2xl />
  <span>Cost of Using a Tool</span>
</div>

<div grid="~ cols-[max-content_min-content_auto] items-center gap-6" py8 px3>
  <div flex="~ gap-2 items-center" text-blue relative v-click>
    <div w-35px h-45px border="l b gray/30" left-0 bottom-15px absolute />
    <div i-ph-magnifying-glass-duotone text-2xl ml-12/>
    <span>Cost of Discovering</span>
  </div>
  <div i-ph-arrow-right-duotone op50 v-click />
  <div v-after>Common needs, easy to find</div>

  <div flex="~ gap-2 items-center" text-lime relative v-click>
    <div w-35px h-56px border="l b gray/30" left-0 bottom-15px absolute />
    <div i-ph-book-bookmark-duotone text-2xl ml-12/>
    <span>Cost of Learning</span>
  </div>
  <div i-ph-arrow-right-duotone op50 v-click />
  <div v-after>Easy to understand and get started</div>

  <div flex="~ gap-2 items-center" text-amber relative v-click>
    <div w-35px h-56px border="l b gray/30" left-0 bottom-15px absolute />
    <div i-ph-currency-circle-dollar-duotone text-2xl ml-12/>
    <span>Price</span>
  </div>
  <div i-ph-arrow-right-duotone op50 v-click />
  <div v-after>Usually free in Open Source! 💛</div>

  <div flex="~ gap-2 items-center" text-orange relative v-click>
    <div w-35px h-56px border="l b gray/30" left-0 bottom-15px absolute />
    <div i-ph-plugs-duotone text-2xl ml-12 />
    <span>Cost of Adoption</span>
  </div>
  <div i-ph-arrow-right-duotone op50 v-click />
  <div v-after>Provide integrations, extensibility</div>
</div>

<!--
So, here we know that we should probably reduce the "Cost of using a tool" to make it easier for ppl to pick up.

[click] From my point of view, the cost of a tool is composed by the following factors.

[click] The first one is the "Cost of Discovering". [click] It's about how commonly for people to realize they need to find a tool for a certain task. It also means the tool should be well-described so that people can easily get what the tool is for with one or two sentences.

[click] Then we have the "Cost of Learning". [click] This is a particularly important one in my opinion. It's about how easy for people to understand and get started with the tool. As the tool is supposed to be used and to make the actual work easier, we certainly don't want users to struggle on learning it for too long before they can be benefited from it.

[click] And then we have the "Price". The cost of the tools itself. [click] We are lucky that in Open Source, the majority of the tools are free to use. Thanks to every maintainer and contributor behind the scenes and making so much awesome tools for everyone to use. And of course, on the other hand, if the tool is not free, this is definitely one of the factors that users would consider on choosing.

[click] And the last one is the "Cost of Adoption". [click] Like how to install and integrate into ones project, how extensible the tool is for potential future needs, how migration would cost, etc.

All those factors are introduced because of the use af an external tool. In the end, we want to see the cost of the tool to be paid off by the benefits it provides.

We know that the complexity of things might transfer from one place to another, but not going to magically disappear. If we are solving a complex problem, it would be honestly hard to prevent the tool from getting complex too. For that, what I learned from the popular open source tools out there is something called "Progressive".
-->

---
glow: bottom
---

# What is Progressive?

<div text-white:50 v-click="5">
The <span v-mark.box.teal.delay400="5" text-teal mx1>"Stairs"</span> to make things easier to approach</div>

<div absolute w-50 h-100 left-34 top-61 v-click>
  <img
    src="/progressive-anthony-char.png" absolute w-50 left-0 top-0 transition duration-500 class="origin-[35%_50%]"
    :class="$clicks === 3 ? 'scale-x--100' : $clicks > 3 ? 'forward:delay-400' : ''"
  />
  <img src="/progressive-mark-question.png" absolute w-12 left--4 top--12 v-click="[3,4]">
  <img src="/progressive-mark-bulb.png" absolute w-20 left-23 top--16 forward:delay-800 v-click="4" >
</div>

<div absolute w-230 right-0 top-5>
  <img
    src="/progressive-floors.png" duration-400
    v-click
    :class="$clicks >= 4 ? 'duration-700 forward:delay-200 op10' : ''"
  />
  <img src="/progressive-stairs.png" duration-400 absolute left-0 top-0 v-click="4">
</div>

<!--
So, after this long intro, finally we are back to our topic today - what's is Progressive?

I think progressive a self is pretty self explaining. But here let's take a quick example with illustrations:

[click] So this is me, [click] and I am trying to get from the first floor to the second. But unfortunately, I hit a wall. The only way to get to there is to jump through the wall. But I'm not a very sports person, so I'm not able to jump that high. In case I might end giving up and turn back around. [click] That's a shame because I failed to accomplish what I aiming for because it's too hard.

So from a progressive perspective, I think that's why stairs has been invented.

[click] It allows me to take multiple smaller steps to going upward, and eventually achieve a certain goal that will be very hard to reach without it.

[click] So here, my interpretation to progressive is that the "stairs" to make things easier to approach.
-->

---
glowX: 50
glowY: 130
class: flex flex-col items-center justify-center
title: Vue
---

<div text-center absolute left-1 right-1 transition-all duration-400 op75 ease-in-out :class="$clicks <= 0 ? 'scale-250 bottom-50%' : 'bottom-5'">
<span op50>https://</span>vuejs.org
</div>

<div i-logos-vue text-5em mt--10 />
<h1 v-click forward:delay-400 text-transparent text-center important-text-5xl font-800 important-leading-1.2em style="background: -webkit-linear-gradient(315deg,#42d392 25%,#647eff);-webkit-background-clip: text;">The Progressive<br>JavaScript Framework</h1>
<div v-click text-xl op75>
"A framework that can grow with you and adapt to your needs."
</div>

<!--
Let's take some real world examples of how progressive works in our daily tools.

If you go to the official Vue documentation, vuejs.org. [click] You see the headline describe itself as the progressive JavaScript framework. And inside the docs, [click] there's a statements mention that Vue is a framework that can grow with you and adopt with your needs.

I have heard people saying that one of the main selling points of Vue is that Vue is very easy to learn and get started. And more than that, I also see Vue is awesome because it can be used in basically everywhere thanks to the progressive approach it takes.
-->

---

# Progressive on Integrations

Vue offers multiple ways to use, for different level of integrations:

<div pt3 />

<v-clicks>

- CDN without build tools

- As Web Components
- Single-page application (SPA)
- Static site generation (SSG)
- Server-side rendering (SSR)
- Native targeting
- Vue Vapor Mode <sup op50 italic font-serif>Coming soon</sup>

</v-clicks>

<!--
Vue is progressive on integrations. Vue provides multiple builds and offers many ways to use in different scenarios.

[click] Like you can use Vue with a single line of CDN import, and enhance your web apps even in a static HTML file without any build tools.

[click] You can also use Vue components as Web components so that's it can coexist with the other frameworks. Vice versa you can also import web components within Vue applications.

[click] When we have build tools set up, we can build Vue applications with Vue single file components that colocate necessary context inside a single file. To build interactive single page application with ease.

[click] With tools like VitePress, it allows you to have efficient static side generation that ships minimal JavaScript while retains a great developer experience.

[click] With tools like Nuxt, we could have server-side rendering with Vue to maximize the end-user experience as well as better SEO results.

[click] Native targeting it also possible via Ionic or NativeScripts.

[click] And then we have the upcoming Vapor mode, which allows components to opt-in a more performance VNode-less render engine to optimize even further in performance critcal scenarios.
-->

---
layout: center
class: text-center
title: Levels of Integrations
---

<h1 important-text-5xl>Levels of Integrations</h1>

<h3 v-click text-white:50>Cover different scenarios, coexist with other techs, <span text-1.4em font-hand text-blue v-mark.highlight.delay400="{at:1,color:'#60a5fa20'}">easy to adopt</span></h3>

<!--
Vue's approach provides the progressive on the levels of integrations.

Allows it to cover the needs for different scenarios, or even coexist with other technologies. [click] This means even you have a large codebase using other stacks but want to use Vue, you can still adopt some parts of you app to use Vue first, and gradually migrate each part slowly. As far as I know, for example, [Wikimedia also picked Vue](https://lists.wikimedia.org/hyperkitty/list/wikitech-l@lists.wikimedia.org/thread/SOZREBYR36PUNFZXMIUBVAIOQI4N7PDU/) and started enhancing with Vue.

In the end, the goal is to make our tool easy to adapt for different levels of needs so we could serve a wilder range of the users.
-->

---
glowX: 50
glowY: 130
class: flex flex-col items-center justify-center
title: Nuxt
---

<div text-center absolute left-1 right-1 transition-all duration-400 op75 ease-in-out :class="$clicks === 0 ? 'scale-250 bottom-50%' : 'bottom-5'">
<span op50>https://</span>nuxt.com
</div>

<div i-logos-nuxt-icon text-5em mt--10 />
<h1 v-click forward:delay-400 text-center important-text-5xl font-800 important-leading-1.1em>The Intuitive<br><span text-hex-00dc82>Vue Framework</span></h1>
<div v-click text-xl op75>
"To make web development intuitive and performant with a great Developer Experience"
</div>

<!--
And then, let's talk about Nuxt.

If we go to nuxt.com, [click] we will see it's titled as "The Intuitive Vue Framework". And in the docs, it mentions [click] Nuxt's goal is "To make web development intuitive and performant with a great Developer Experience".

And that brings us to the next section, "Progressive on Onboarding".
-->

---
glow: bottom
---

# Progressive on Onboarding

<div v-click text-white:50 mt5>
This is <b text-white:75>all you need</b> to start with Nuxt:
</div>

<div grid="~ cols-2 gap-x-2" mt5>
<div flex="~ gap-2 items-center" v-click="2">
  <div i-logos-npm-icon />
  package.json
</div>
<div flex="~ gap-2 items-center" v-click="3">
  <div i-logos-vue />
  app.vue
</div>

<div v-click="2">

```json
{
  "scripts": {
    "dev": "nuxt dev",
    "build": "nuxt build"
  },
  "devDependencies": {
    "nuxt": "^3.10.0"
  }
}
```

</div>
<div v-click="3">

```vue
<script setup>
const msg = ref('Hello, Nuxt!')
</script>

<template>
  <h1>{{ msg }}</h1>
</template>
```

</div>
</div>

<div mt10>
<span text-2xl v-click="4">Intuitive</span> <span op50 v-click="5"> - Minimal knowledge required, and easy to discover new features</span>
</div>

<!--
If you have ever tried Nuxt's starter template - you will find it's surprisingly easy to start a Nuxt app. [click]

All you need is to have `nuxt` installed as your dev dependencies [click], and create a simple Vue component file as `app.vue`. [click]

And that's it, that's all you need to get start with Nuxt. Even to someone who never tried Vue or Nuxt, it's probably not hard to tell what this will render, or how to modify it, as long as they get the basic idea of what is HTML.

[click] I think Nuxt's "Intuitive" here [click] means that you can get started with very minimal knowledge. While also, it should be fairly easy to enable more features as needed.
-->

---

# Progressive on Features

<div v-click text-white:50 mt3 mb6>
Starts <b text-white:75 font-bold>minimal</b> and <b text-white:75 font-bold>grows</b> with users:
</div>

<!--
<div v-click mt-20 mb-4 op75>
By the minimal starting interface, Nuxt allows you to start with a minimal setup and grow with the features you need.
</div>

<div flex="~ gap-4" text-white:75>
<v-clicks>

  <div flex="~ gap-1 items-center">
    <div i-ph-circle-wavy-check-duotone text-xl text-lime />
    Server-side Rendering
  </div>

  <div flex="~ gap-1 items-center">
    <div i-ph-circle-wavy-check-duotone text-xl text-lime />
    Deploys Everywhere
  </div>

  <div flex="~ gap-1 items-center">
    <div i-ph-circle-wavy-check-duotone text-xl text-lime />
    Ecosystem of Nuxt / Vue / Vite
  </div>

  <div flex="~ gap-1 items-center">
    <div i-ph-circle-wavy-check-duotone text-xl text-lime />
    Serverless APIs
  </div>

</v-clicks>
</div>
-->

<div flex="~ col gap-6">

<div flex="~ gap-2 items-center">
  <div flex="~ gap-2 items-center" v-click>
    <div i-ph-circles-three-plus-duotone text-2xl />
    <span font-bold>Have some components?</span>
  </div>
  <span v-click op75 ml4>Put them in <code>components/</code> and use anywhere</span>
</div>

<div flex="~ gap-2 items-center">
  <div flex="~ gap-2 items-center" v-click>
    <div i-ph-signpost-duotone text-2xl />
    <span font-bold>Need routing?</span>
  </div>
  <span v-click op75 ml4>Create a <code>pages/</code> directory and Vue router is set up for you.</span>
</div>

<div flex="~ gap-2 items-center">
  <div flex="~ gap-2 items-center" v-click>
    <div i-ph-cloud-arrow-up-duotone text-2xl />
    <span font-bold>Deploy your site?</span>
  </div>
  <span v-click op75 ml4 flex="~ items-center gap1">It <span text-green>Just works™</span> with zero-config powered by <img src="/nitro.svg" h-1.3em /><span text-purple>Nitro</span></span>
</div>

<div flex="~ gap-2 items-center">
  <div flex="~ gap-2 items-center" v-click>
    <div i-ph-cloud-duotone text-2xl />
    <span font-bold>Need some server logic?</span>
  </div>
  <span v-click op75 ml4>Create a <code>server/api/</code> directory to make serverless endpoints.</span>
</div>

<div flex="~ gap-2 items-center">
  <div flex="~ gap-2 items-center" v-click>
    <div i-ph-file-ts-duotone text-2xl />
    <span font-bold>Want TypeScript?</span>
  </div>
  <span v-click op75 ml4>Oh, you can just use it!</span>
</div>

<div flex="~ gap-2 items-center">
  <div flex="~ gap-2 items-center" v-click>
    <div i-ph-puzzle-piece-duotone text-2xl />
    <span font-bold>PWA, SEO, i18n, RSS, etc?</span>
  </div>
  <span v-click op75 ml4>We have great modules ecosystem to use in a few clicks.</span>
</div>

<div flex="~ gap-2 items-center">
  <div flex="~ gap-2 items-center" v-click>
    <div i-ph-cat-duotone text-2xl />
    <span font-bold>Curious about more?</span>
  </div>
  <span v-click op75 ml4 flex="~ items-center gap1">We have <div i-logos-nuxt-icon text-xl inline-block/><span text-green>Nuxt DevTools</span> to inspect and analyze the internals</span>
</div>

</div>

<!--
Then let's talk about one other aspect that Nuxt is good at - Progressive on features.

So we know that Nuxt works with a bare minimal starter, be also we know a real-world application won't be that simple. We need a lot capability to accomplish various needs, and also a way for us to organize the codebase in an managable way.

[click] Nuxt is the framework that can grows with your need!

[click] To say, if you want to some components to separate and reuse your logic, [click] in Nuxt you can just create components files under the components directory, and they will be auto-discoverabale across your project.

[click] And then if you our app needs the capability to serve multiple pages and do the navigations, [click] you can create the `pages/` directory. The components under it will be register automatically to your router based on their filename. One of the other great part is that until you do this, `vue-router` or related code were never ships to your production app before you actually using it.

[click] Say our app is now ready to go, we want to deploy the site to somewhere. There are quite many deploy platform you can choose from, and usually you will need to learn a bit how to deploy X framework on Y platform, etc. [click] But with Nuxt, they will just works on all major hosting services with zero config, thanks for the automatic deploy presets powered by Nitro.

[click] It's common for an web app to have some server logics and API end points. [click] In Nuxt you can simply create function modules under `server/api` directory, witha a very similar convention like the pages for routing. Nitro will deploy them in the serverless functions based on your hosting services and we have the end-to-end type safety on developement.

[click] Talking about type safety, if later you learned TypeScript and want to use it with in Nuxt - [click] no problem, you can directly use them as Nuxt already understand it.

[click] For more features like Progressive Web Apps, Search engine optimization, internationallizations, etc. [click] Nuxt provides a rich module ecosystem that you can integrate them within a few clicks.

[click] And finally, in case you are interested in more features Nuxt provides, [click] we also built Nuxt DevTools for you to inspect the internals or analyze your apps.

All those features are opt-in, meaning that if you don't need a certain feature, you don't even need to learn it. And once you find it useful later, you can always grab it back easily.
-->

---
class: grid grid-cols-[auto_640px] gap-4 items-center justify-center
glow: left
---

<div flex="~ col gap-4">
<div text-4xl>Nuxt DevTools</div>
<div op50 v-click>Help features discovery<br>and understanding</div>
</div>

![](/nuxt-devtools.png){.my--10}

<!--
To help with the features discovery, we made Nuxt DevTools as we just mentioned.

For example, DevTools provides a modules tab, that you can have a quick overview of how many modules you have installed, with links to their documentations or the source code repo. It also offers you a nice UI for you to search through all the modules across the community, and you can ask DevTools to automatically download them and install for you with a single click.

[click] DevTools is built to help features discovery and understanding, to assist you crafting even more awesome applications.
-->

---
class: grid grid-cols-[640px_auto] gap-6 items-center justify-center
glow: right
---

![](/nuxt-tutorial.png){.my--10}

<div flex="~ col gap-4" text-right>
<div text-4xl>Nuxt Tutorial</div>
<div op50 v-click>Help onboarding<br>and learning</div>
</div>

<!--
On top of the documentation site Nuxt has, in the past months we started to build an interactive tutorial playground. Some of you here probably have watched my live streaming on building it, thank you for working together with me btw.

So Nuxt Tutorial allows beginners to have a more linear, step-by-step learning experience. So they can start playing with Nuxt more easier without the need to install or setup.

[click] This is another case that we are trying to get the progressive onboard experience even smoother.
-->

---
layout: center
class: text-center
---

<h1 important-text-5xl>Grow with Users</h1>

<h3 v-click><span op50>Expose concepts & powers </span><span text-lime font-hand text-4xl v-mark.underline.lime.delay400="1">progressively</span></h3>

<!--
In short, the point here is that we should grow with users and not putting too much stuff upfront at one.

[click] Make learning easier to starts with, and expose new concpets and powers progressively along the way.
-->

---
glowHue: 100
class: flex flex-col items-center justify-center
---

<div text-center absolute left-1 right-1 transition-all duration-400 op75 ease-in-out :class="$clicks === 0 ? 'scale-250 bottom-50%' : 'bottom-5'">
<span op50>https://</span>vitejs.dev
</div>

<div i-logos-vitejs text-5em mt--10 mb2 />
<h1 v-click forward:delay-400 text-center important-text-5xl font-800 important-leading-1.1em>Next Generation<br><span text-purple>Frontend Tooling</span></h1>
<div v-click text-xl op75>
"We work closely with projects in the ecosystem to minimize regressions on each release"
</div>

<!--
And then, let's take one more example, Vite.

[click] Vite titled itself as the next generation frontend tooling. I am prettry sure no one would question that.

[click] In the "Vite philosophy" section, the docs mentions that "Vite works closely with projects in the ecosystem to minimize regressions on each release".

Vite is on major version 5 right now. And during the past 4 years, we basically keep the pace of release 1 major version per year to keep up the JavaScript ecosystem and the evolving standards.

Some of you probably have been through that periods where we do major releases. The last one with Vite 5 and was released on November last year.

It's not a secret that Vite's major releases have very smooth migration paths. We received many comments mentions about their successful migrations cases.
-->

---
glowHue: 90
glow: top-right
class: flex items-center justify-center
---

<div relative>
  <Tweet id="1547266714466861056" ml--45 mt--4 flex justify-center items-center transition class="important:[&_iframe]:w-230 important:[&_iframe]:rounded-13px" :class="$clicks > 1 ? 'op50 duration-600' : ''" v-click />

  <Tweet id="1725177397949944126" absolute top-15 left-5 class="important:[&_iframe]:w-200 important:[&_iframe]:rounded-13px important:[&_iframe]:shadow-xl" v-click />
</div>

<!--
[click] Project monorepo mention that they upgraded Vite 2 to Vite 3 with only bumpping version, everything keeps working as-is.

[click] Kilian even describe Vite as the "Most painless full-version upgrade of a build system ever" on the release of Vite 5.

And many more comments like this. Thank you and we are glad to hear those stories.
-->

---
glowHue: 60
glow: right
class: flex flex-col items-start justify-center
---

## A Typical Vite Plugin

<div mt5 v-click>
<div flex="~ gap-2 items-center">
  <div i-logos-npm-icon />
  package.json
</div>

```json
{
  // ...
  "peerDependencies": {
    "vite": "^2.9.0 || ^3.0.0 || ^4.0.0 || ^5.0.0"
  }
}
```

</div>

<div mt4 relative>
<span v-click>The plugin keeps working from <span v-mark.underline.purple="3">Vite 2 to Vite 5</span></span>
<img src="/vite-3years.png" absolute left-65 top-10 rotate-10 w-33 alt="3 years in between" v-click />
</div>

<!--
If you look into the Vite plugins you are using, you will find many of their `package.json` follow a similar pattern like this:

[click] Vite appears in the `peerDependencies`  with the version range from Vite 5 all the way down to Vite 2.

[click] This means that the plugin keeps working from Vite 2 to Vite 5 perfectly without the need to even drop support of the previous Vite versions.

[click] Not to mention there is 3 years of time in between, for such an active tool like Vite.

Vite team has put a lot of care in it to make this possible. We care a lot about every changes we made, that we even work out the idea of "Ecosystem CI" that runs the test of major downstream frameworks on almost every pull requests to make sure they has the minimal impact to the ecosystem. This practice has been later adopted to Vue, Nuxt and many other frameworks.

And that brings up one other aspect of progressive.
-->

---
glow: right
---

# Progressive on Breaking Changes

<p v-click="3">Two ways of make breaking changes easier</p>

<div absolute left-29 top-35 w-80 transition duration-800 v-click="1" :class="$clicks <= 3 ? 'translate-x-50 translate-y-10 scale-150' : '' ">
  <img src="/breaking-changes-floors.png" absolute inset-0 op75>
  <div font-hand absolute left-0 top-39 text-2xl>v1.0</div>
  <div font-hand absolute left-23 top-12 text-2xl v-click="7" text-yellow>v1.x</div>
  <div font-hand absolute right-0 top--6 text-2xl transition duration-800 :class="$clicks >= 10 ? 'translate-x--22 translate-y-25 text-blue' : ''">v2.0</div>
  <div font-hand absolute right-0 top--6 text-2xl text-orange v-click="10">v3.0</div>
  <img src="/breaking-changes-stairs-right.png" absolute inset-0 v-click="3">
  <img src="/breaking-changes-stairs-left.png" absolute inset-0 v-click="2">
</div>

<div absolute left-15 bottom-10 transition duration-800 :class="$clicks <= 3 ? 'translate-x-20 translate-y--13  scale-120' : '' ">
<div flex="~ gap-2 items-center" text-yellow3 mt-8 mb2 text-xl v-click="2">
  <div i-ph-escalator-down-duotone text-2xl scale-x--100 />
  <span>Forward Compatibility</span>
</div>

<v-clicks at="5">

- Compatible with the [future]{.text-yellow.font-bold} versions
- Introduce the `experimental` or `future` flags
- Make future behavior opt-in today
- (e.g. `@vue/composition-api`, `vue v2.7`, [Nuxt Bridge](https://github.com/nuxt/bridge))

</v-clicks>
</div>

<div absolute left-120 top-30 transition duration-800 :class="$clicks <= 3 ? 'translate-x-35 translate-y-35 scale-120' : '' ">
<div flex="~ gap-2 items-center" text-blue mt-8 mb2 text-xl v-click="3">
  <div i-ph-escalator-up-duotone text-2xl />
  <span>Backward Compatibility</span>
</div>

<v-clicks at="9">

- Compatible with the [previous]{.text-blue.font-bold} versions
- Deprecate first, print warnings, remove later
- (e.g. `@vue/compat`, `@nuxt/kit`)

</v-clicks>
</div>

<!--
Progressive on Breaking Changes.

I guess probably no one likes breaking changes. But somehow breaking changes are also quite important for the codebase to stay healthy and more maintainable in the long run. It help us to fix imperfectness of our previous design, with a better context we have today. While it's had to avoid introducing them, I believe maybe there would be some ways to make it the transition smoother and easier for the users to adopt.

[click] Taking the experience we had in Vue and Vite, I see there are two major ways to achieve that. Here we bring back the graph we had before, refering to the jump between major versions 1 and 2.

[click] One way of make breaking changes progressively is to do Forward Compatibility, [click] and the other is Backward Compatibility. Let me explain. [click]

[click] Forward Compatibility is about to compatible with versions in the future, like to say if you know what's the new features you going to have in the next breaking change, you bring the features back to the current version in a non-breaking way.

[click] In practice, often we will introduce flags such as `experimental` or `future` for users [click] to explicitly opt-in those changes if they want to try the new stuff, while the mainstream of the users can still be on the current version without breakages.

[click] In Vue, we have the example of `@vue/composition-api` plugin back in Vue 2, which provide the capability of using Vue 3's composition API for Vue 2 apps before they can migrate to Vue 3.

And later we have Vue v2.7, 2 years after Vue 3.0 has released, to have composition API support bake in, and align more with Vue 3's behaviour and feature sets.

For Nuxt, we introduced Nuxt Bridge, to briging the changes betwen Nuxt 2 and 3.

[click] Then it's take about Backforward compatibility, which you might heard this more often. It's about to be compactible with the previous versions.

[click] A common practice is that we will mark a certain feature as deprecated, that will print warnings upon usage. And eventually removed later in the next major version or so. This also means it's better to do smaller and a bit more frequent major releases to make the migration easier.

[click] Talking about examples, in Vue we have the compatibility build, that use Vue 3 as the fundation but with additional flags to simulate the legacy Vue 2 behaviour. That you can migrate once a feature. On Nuxt we have Nuxt Kit that allows module aurthor to build modules that would in both Nuxt 2, Bridge and Nuxt 3. etc.
-->

---
layout: center
class: text-center
glowX: 50
glowY: 0
---

<h1 important-text-5xl>Allow Coexistence</h1>

<h3 v-click text-white:50>Provide <span text-orange v-mark.underline.orange.delay400.op75="1">"middle stages"</span> for migration, coexist of legacy & new</h3>

<!--
From my understand, I think the progressive of breaking changes is fundamentally allowing the co-existence.

[click] When we make changes, we should provide the "middle stages" for ppl to take a rest on migration, allowing the coexistence of both legacy and new. So the work can be done progressively, and reduce the chance of breakages.
-->

---
glow: right
---

<!--

# Extensible Plugins System

- Allows community to progressively enhance the tool and enrich the ecosystem -->

# Recap

<div flex="~ col gap-1" pt6>

<div text-xl text-white:50 v-click>
Progressive on <span flex="inline gap-1 items-center" text-lime translate-y-0.6><div i-ph-book-bookmark-duotone />Onboarding</span>
</div>
<div flex="~ gap-2 items-center" mb3 ml37 v-click>
  <div i-ph-arrow-bend-down-right-duotone op50 />
  <div>
    Making it easy to understand and get started
  </div>
</div>

<div text-xl text-white:50 v-click>
Progressive on <span flex="inline gap-1 items-center" text-purple translate-y-0.6><div i-ph-puzzle-piece-duotone />Integrations</span>
</div>
<div flex="~ gap-2 items-center" mb3 ml37 v-click>
  <div i-ph-arrow-bend-down-right-duotone op50 />
  <div>
    Fits in different scenarios, easy to adopt
  </div>
</div>

<div text-xl text-white:50 v-click>
Progressive on <span flex="inline gap-1 items-center" text-yellow translate-y-0.6><div i-ph-lightbulb-filament-duotone />Features</span>
</div>
<div flex="~ gap-2 items-center" mb3 ml37 v-click>
  <div i-ph-arrow-bend-down-right-duotone op50 />
  <div>
    Starts minimal and grows with users
  </div>
</div>

<div text-xl text-white:50 v-click>
Progressive on <span flex="inline gap-1 items-center" text-rose translate-y-0.6><div i-ph-warning-octagon-duotone />Breaking Changes</span>
</div>
<div flex="~ gap-2 items-center" mb3 ml37 v-click>
  <div i-ph-arrow-bend-down-right-duotone op50 />
  <div>
    Provide middle stages for migration
  </div>
</div>

</div>

<!--
So, to recap today's topic, we have talked the progressiveness on different aspects of building a tool.

[click] The first is about progressive on onboarding, [click] we should make the tool easy to learn and understand, for more people to start benefited from the tool we build.

[click] And then we talked about the progressive on integration [click] for our tool to cover different scenarios, and easy to adopt.

[click] Then we have the progressive on features, it's pretty common that we want to make our very powerful but that could be overhelming for the users to starts with. [click] So, taking the progressive approach would allows us to start minimal and grow with the users.

[click] And then finally, we have progressive on breaking changes, [click] to provide middle stages to make migrations step by step.
-->

---
layout: center
class: text-center
glowX: 50
glowY: 0
---

<h1 important-text-5xl>Progressive Paths</h1>

<h3 v-click text-white:50>Enables users the capability of <span text-lime font-bold v-mark.highlight.lime.op5.delay200="1" inline-block p3 mx--2>"Divide and Conquer"</span></h3>

<!--
There are much more aspects of progressiveness that we didn't have time to talk about today, but my goal today is to bring this idea of "Progressive Path" to you.

It might not seems to be a very cool or unusual stuff that people would get excited about, but I think it is playing a very important role to our daily software development. And we should think about it more often when building stuff, not only for open source projects, but also probably also for your products, or the ways of doing stuff in general.

[click] To finish my talk with one sentence, I'd say "To provide the progressive paths, is to enable users the capability of 'Divide and Conquer' towards the goals they have".

I hope you enjoy and find it useful.
-->

---
layout: intro
class: text-center pb-5
glowX: 50
glowY: 120
---

# Thank you!

Slides on [antfu.me](https://antfu.me)

<!--
That's all for my talk, thank you, and happy hacking!
-->
