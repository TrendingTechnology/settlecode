+++
categories = ["Javascript"]
date = 2019-12-15T16:00:00Z
description = "In this article, we'll explore what the JAMstack is and what's so good about it, as well as check out some of the best NodeJS-based Static Sites Generators (SSGs). Let's get started!"
featuredimage = "https://res.cloudinary.com/diqqalzsx/image/upload/v1576509790/content/settlecode/JAMStack_hv3ybg.jpg"
slug = ""
tags = ["JAMStack"]
title = "How to Generate Static Sites With Javascript Static Sites Generators"

+++
_Static websites_ and so-called _JAMstack_ have become pretty popular recently. And with 2020 on the horizon, this trend doesn't seem to be stopping. Why? Why is old-school HTML + CSS + JS trio in its redesigned and renamed form gaining so much attention? In this article, we'll explore what the JAMstack is and what's so good about it, as well as check out some of the best NodeJS-based Static Sites Generators (SSGs). Let's get started!

## [**JAMStack**](https://jamstack.org/)

![The JAMStack](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509856/content/settlecode/jamstack_1_omknum.jpg)

For starters, let's talk a bit about the JAMstack and static websites themselves. As you might already know, _stack_ in programming is a term used to reference some _toolset_ - a collection of libraries and frameworks. The popular examples of that are _MEAN_ (_MongoDB_, _ExpressJS_, _Angular_, and _NodeJS_) and _MERN_ (_React_ instead of Angular) stacks. So, as you can see, there's some decrypting going on here.

Now, let's get back to the JAMstack and, more specifically, to its definition:

> Modern web development architecture based on client-side JavaScript, reusable APIs, and prebuilt Markup.

I think the text above is self-explanatory. With this information, we can make sense of the _JAM_ shortcut:

* _JavaScript_ - web developer's best friend, a place where all the logic is executed. Usually present both on the generator and client-side;
* _APIs_ - providers for JS to pull data from;
* _Markup_ - templates, processed at deployment time of your website.

"JAMstack", as a term, was first used by [**Netlify**](https://www.netlify.com/blog/2015/11/16/what-is-the-jamstack/) around 2015. Its primary purpose was to convince developers to well-known and somewhat disliked static websites. A new name was meant to change people’s mindsets about old technology. As we know today - this strategy worked!

The main idea behind the JAMstack is the removal of any tight connection between the client and the server. The only way to receive your data is through _APIs_. Such data can be later processed together with markdown and other resources to create a static website that is then served to the client.

## Reasoning

Now that we know all the terminology, it's time to explore the reasons and benefits behind the JAMstack.

### Pricing

_Pricing_ is probably one of the most important advantages of static websites. To host them, you need no powerful server, _no CMS_ and, what comes with it, _less money_. Remember, you process/prebuild your website to the form of static assets (HTML, JS, CSS, text files, etc.). These can be served ridiculously cheaply with no higher demands than just standard, low-priced hosting.

### Performance

_Performance_ is the next focus point of static websites. This might seem pretty obvious - static assets are fast - it's in their nature. Nothing can beat them in this category. Using JAMstack, you can easily achieve _high Google Lighthouse scores_, thus getting higher in search results too! Outside from that comes the ease-of-use of _Content Delivery Networks_ (CDNs_)_, which can boost your website's delivery speed even more!

### Stability & confidence

This one might be a little tricky. What does _confidence_ mean? Well, mainly the _stability_ of your website and its _architecture_. With JAMstack, things are really straightforward. There's nothing more to it than just the _static frontend_ and the generation process.

Your data comes from different APIs. Other functionalities can be provided with _serverless_ systems. The main idea behind it is that you use _3rd party APIs and services_ to provide additional features to your website. There are many public serverless providers, including [**AWS**](https://aws.amazon.com/), [**Google Cloud**](https://cloud.google.com/), and [**Microsoft Azure**](https://azure.microsoft.com/), all of which play nicely with static websites.

### Scalability

JAMstack-based websites are easily _scalable_. It's mainly due to the performance and architecture solutions behind them. Earlier mentioned, CDNs play an essential role here. Improving the delivery process can mean nothing more than providing more faster CDNs.

### SEO

Yet another holy grail of static websites. When using JAMstack, having good _SEO_ ranking is much easier than with _Single Page Applications_ (SPAs). Static websites get better [**Lighthouse**](https://developers.google.com/web/tools/lighthouse) scores and are more likely to be fully _indexed_ by Google and other search engines. That's where SPAs are truly lacking. You have to use _Server-Side Rendering_ (SSR) to get the same SEO performance as static websites provide pretty much out-of-the-box.

### Security

Last but not least, there are _security_ reasons. With your what could be backend spread into the number of _APIs_ and other 3rd party services, the risk of severe security issues is significantly reduced.

## Downsides

Of course, static websites have some disadvantages too. Probably the biggest one being that they are _static_. Again, what it means is that you don't have any real backend running behind them. And, as not every functionality can be well-substituted by serverless services, JAMstack isn't suitable for everyone.

Furthermore, static websites are not as "upgradable" as their dynamic counterparts. To update their content, you need to _pre-process_ it first. And, the more and more pages your website has, the slower this process becomes. That's why the build performance that many tools advertise so much is so important.

So, with all that said, the decision is yours to be made. Whether you'll choose the static or dynamic path for your future website, it's always good to first consider the pros and cons of both solutions.

## Tooling

Now it's time to explore some of the best JAMStack tools. But before that, let me provide some general details over the following generators.

First, the tools listed below are based on _NodeJS_ (_JavaScript_) and grouped by the used _JS framework_. Second, all the tools here are general-purpose - no documentation generators or other specialized libraries and frameworks.

## React-based

### [**GatsbyJS**](https://www.gatsbyjs.org/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509893/content/settlecode/gatsby_t7fphi.jpg)

_GatsbyJS_ is arguably one of the most popular static websites generators out there. It allows you to utilize popular tools like [**Webpack**](https://webpack.js.org/) and, most importantly, _React_ to create stunning-looking static websites. Besides that, the build speed of GatsbyJS is fast enough to handle even complex, multi-page setups. Great _community_, docs, and vast _ecosystem_ make this generator one of the best in its category. A great number of _plugins_ (both first and third-party ones) allow you to pull data from countless sources (with the help of [**GraphQL**](https://graphql.org/)) and add different functionalities to your website with ease.

### [**Next.js**](https://nextjs.org/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509910/content/settlecode/next_fymv0g.jpg)

_Next.js_ is yet another React-based SSG. It's created and supported by [**Zeit**](https://zeit.co/) and is well-known within the React community. Not only it's a generator but a full-blown framework with other functionalities such as _SSR_ built-in. It gives you a choice on what type of website you want to create. With that said, Next.js can be considered an _All in One_ (AiO) tool for everything that has something to do with React-powered websites. It has excellent _documentation_ and an even better _community_ behind it.

### [**React Static**](https://react-static.js.org/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509921/content/settlecode/react-static_vxtiwr.jpg)

_React Static_, as the name implies, is a progressive _Static Site Generator_ (SSG) for React. Being tightly connected with React, it has great support for all the related libraries and tools, such as [**Redux**](https://redux.js.org/). It has a great build and resulting website performance. It also simplifies the development experience with _hot-reloading_ out-of-the-box. All this and more is documented in fine-tuned GitHub-based docs.

## Vue-based

### [**Gridsome**](https://gridsome.org/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509932/content/settlecode/gridsome_gunbmh.jpg)

Starting the list of _Vue-based SSGs_, we have _Gridsome_. It's somewhat like a _GatsbyJS counterpart_ but for Vue! It has equally impressive build and resulting website _performance_, _Progressive Web Applications_ (PWAs) and _SEO optimizations_ support, and other JAMstack goodness! Maybe it doesn't have the community as big as GatsbyJS has, but, as it's a relatively new project, I think it looks great! With that said, its _documentation_ and community involvement are truly impressive.

### [**Nuxt.js**](https://nuxtjs.org/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509943/content/settlecode/nuxt_pwzjj4.jpg)

_Nuxt.js_ is a _full-blown framework_. What does it mean? Mostly that it's a Next.js Vue alternative and that it has as much as three rendering modes: _SSR_, _static website_, and _SPA_. Nuxt.js as _AiO_ solution allows you to choose what's the best for your website. It's very stable, well-known, and has great _docs_, _community_, and _ecosystem_. With all that in mind, it's the right choice for any kind of demanding Vue project.

### [**VuePress**](https://vuepress.vuejs.org/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509952/content/settlecode/vuepress_nm9r2h.jpg)

_VuePress_ is a little bit different than previous tools. It's very minimalistic and allows you to generate your page's content with the help of simple _markdown_ files. It features rich _plugin architecture_ and leverages the power of _the Vue ecosystem_. It is somewhat tailored towards documentation websites; however, with the option of using custom Vue components in your content, this tool can be used for many different purposes. In general, its main pros are _simplicity_ and _ease-of-use_.

## Other

### [**Hexo**](https://hexo.io/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509962/content/settlecode/hexo_ezw9xi.jpg)

_Hexo_ is NodeJS and _Markdown-based_ SSG, tailored towards _blog writers_. It's fast and has a rich _plugins_ collection. These provide different kinds of features to your Hexo-based static website. The framework also has a well-developed _theme system_ with several themes [**listed**](https://hexo.io/themes/) on its official page. Naturally, you can create your own plugins and themes to suit your personal needs. Hexo also has detailed _documentation_ and a fine-sized community.

### [**Eleventy**](https://www.11ty.dev/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509971/content/settlecode/11ty_sabspi.jpg)

_Eleventy_ (or _11ty_) is a simple SSG, a JS alternative to Jekyll. It's incredibly _flexible_, works well with data, and supports a lot of different templating engines and languages (_markdown_, _html_, [**hbs**](https://handlebarsjs.com/), etc.). 11ty's overall simplicity, ease-of-use, and progressive nature make it a valuable tool. Also, docs are great and very informative.

### [**Sapper**](https://sapper.svelte.dev/)

![](https://res.cloudinary.com/diqqalzsx/image/upload/v1576509980/content/settlecode/sapper_w0x9xs.jpg)

_Sapper_ is an SSG based on the [**Svelte framework**](https://svelte.dev/), that on its own, is recently getting a lot of traction. Because of the nature of Svelte, which moves a lot of processing to the compilation step, it's _fast_ by default. Sapper also has _SSR_ support and other _AiO framework_ goodness. So, if you like Svelte, are interested in it, or want to try it out, then Sapper might be the choice for you.