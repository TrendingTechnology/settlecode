+++
categories = ["JavaScript"]
date = 2019-12-17T16:01:00Z
description = "It's nice to have all this simplicity out-of-the-box, but sometimes you need more."
featuredimage = "https://res.cloudinary.com/diqqalzsx/image/upload/v1576657113/content/settlecode/JavaScript_ru02av.jpg"
slug = ""
tags = []
title = "CodePen vs CodeSandbox - JavaScript playgrounds compared"

+++
As one of 4 languages running on the Web, JavaScript is extremely easy to get started with. Just open your desktop browser, go to the _developer tools_ (usually with _F12_), and that's it! From there, you can play with JS, without installing or running any complicated setup. All you need is a _browser_.

It's nice to have all this simplicity out-of-the-box, but sometimes you need more. For example, you want to play with some new Web API you've just learned, but you don't want to set up a whole new project.

Unless you've got all the boilerplate laying around, you'd most likely have to install and configure everything from the ground-up. Sadly, dev tools and built-in console won't cut it either - they're too basic and thus ill-suited for such a purpose. There's only one solution left - a _coding playground_.

Because of its unique position, JavaScript is the most straightforward language to be run on the Web. Thus, it's the most supported one among online playgrounds - places where you can write and play with code with ease. There are many of them around the Web, but only a few are well-known and trusted.

In this article, we'll check how the two most popular JS playgrounds - _CodeSandbox_ and _CodePen_ - stack against one another in an in-depth comparison. Let's begin!

# [**CodeSandbox**](https://codesandbox.io/)

![CodeSandbox landing page](https://areknawo.com/content/images/2019/12/codesandbox.png)CodeSandbox landing page

Created in 2017 (younger from the two), CodeSandbox is meant to improve and accelerate the web development process. It removes all the complexities related to the project's setup and allows for easy, real-time collaboration.

At the foundation of CodeSandbox are _Sandboxes_ - units containing the actual projects and their code. At the time of writing, there are over 3 million of them, and most of their code is freely available for your own use-cases. With that said, CodeSandbox is also open-source itself, and its codebase is [hosted on GitHub](https://github.com/codesandbox/codesandbox-client).

# [**CodePen**](https://codepen.io/)

![CodePen landing page](https://areknawo.com/content/images/2019/12/codepen-1.png)CodePen landing page

Ever since its introduction in 2012, CodePen has grown into a huge _social development environment_. It focuses on small playgrounds called Pens that can be easily shared, embedded, and grouped whenever and however you want.

Because of its size and the system of posts, comments, and reactions, CodePen surely is an interactive social platform for web developers. Your account there can be used as a beautiful portfolio, a code-heavy blog, and a lot more...

# **Features**

Both playgrounds have a lot in common, but they also have some differences. They focus on different goals and achieve them in their own unique ways.

## **Editor**

In terms of the actual editing space - the place where the magic happens - these two couldn't be more different.

When using CodeSandbox, any project you create starts with a _template_. It can either correspond to a specific library, framework, or runtime (Node.js included), or utilize only vanilla web technologies. After choosing the template, you're moved to the editor with all the necessary files, and the preview window already opened.

All Sandboxes give you access to a "file system", meaning that you can create additional files, use modules (including NPM packages), and interact with static assets. There's also an option to edit the _configuration files_ that are specific to the given template.

The editor itself is powered by the open-source [Monaco Editor](https://microsoft.github.io/monaco-editor/), which you might be familiar with from the _VS Code_. What it means is that all the productivity features (e.g., intellisense and go to the definition) are there to help you.

On the other side of things, CodePen provides you with two "modes". The first and the most used one is the _Pen_. Creating one is as simple as clicking a button, after which you're taken straight to the editor.

From there, you have access to a preview panel and basic HTML, CSS, and JS editing windows. No "file system", intellisense or anything like that - only simple syntax highlighting and quick commands like prettify. In the _settings panel_, you're allowed to choose from a limited set of preprocessors for all three languages (like TypeScript for JS) or add links to external sources.

When comparing CodePen's Pens and CodeSandbox' Sandboxes, based on what we've already covered, you might come to a logical conclusion that CodeSandbox provides more and better features. While it's somewhat true, it's not always what one might want. Remember that playgrounds are mostly used for quick and dirty tests, which simple Pens are pretty good for.

Anyway, if all you're missing in your Pen is "file system" support, then you can go for the CodePen's _Projects_. The editing experience is still similar, but a bit limited in the free version.

## **Social**

Depending on what your goals are, the social features of your playground might or might not be relevant to you. However, both of the discussed tools possess at least some basic functionalities in this field.

In CodeSandbox, you've got some metrics about your Sandboxes' views, likes, and forks count. You've also got an option to set the title, description, and tags for your project. Apart from that, there's a [whole page](https://codesandbox.io/explore) dedicated to exploring and searching through all the public sandboxes.

But, by far the most impressive social feature of CodeSandbox is the _real-time collaboration_. You can start your live session at any time, invite your team and see what everybody's doing. Such a feature is incredibly helpful when working within remote teams.

As I said, CodePen takes social experiences to another level. Likes, comments, views, tags, posts, collections, etc. - it all makes CodePen a _social web development platform_. There's even some room for the job listings, challenges, a newsletter, and the exploration page. Lastly, you get a live collaboration mode, but only if you are opt-in for one of the Pro plans.

## **Others**

Aside from the social experiences and the editor itself, both platforms provide other unique features.

CodeSandbox stands out with its editor's functionalities. You get a dedicated _test runner_, deep _GitHub integration_ (repo import, commits and pull requests) and built-in _deployment tool_ for [ZEIT Now](https://zeit.co/home) and [Netlify](https://www.netlify.com/) (currently in beta).

You also have access to some of VS Code settings. This way, you can configure your _theme_ (can be a custom one), adjust Prettier config, and do other things.

Again, the main focus of CodePen are social features, so it's no surprise that its strength lies there. Take _documentation_ and a _dedicated blog_, for example. Both tools have them, and they're pretty much on pair, but CodePen's docs are a bit more detailed, and its blog is much more active. CodeSandbox's blog focuses mainly on the tool updates and new features, while the CodePen's also touches on things going behind the scenes, with an additional _podcast_ included.

# **Premium**

While you'll most likely use either of these tools for free, it might be important for you to know the differences between them when it comes to the _premium tiers_.

[CodeSandbox](https://codesandbox.io/pricing) is pretty clear in this regard. For _$12_ a month, you're allowed to create unlimited private sandboxes and connect with private GitHub repos. You also get a higher storage limit (counted for all the sandboxes), from 50MB (in free tier) to 500MB. And if you're interested, there's a _Pro plan_ for Teams coming soon.

On [CodePen](https://codepen.io/accounts/signup), you've got a bit more options to choose from. There are three premium plans for _$12_, _$19_ and _$39_ a month or less if you pay annually. Any of the three tiers allows you to create unlimited private pens, posts, and collections. You'll also get the _Pro badge_ (social boost), access to live collab mode, no ads, and more.

There're also some special plans for teams and other cross-tier differences. For that, you can check out the official billing board.

# **Winner**

So, based on what we've already covered, we should be able to pick the winner. But things aren't so straight-forward. One playground is better than another in some regards and vice-versa. We can only decide based on specific categories.

If all you want is to get stuff done for free, either of the editors will do. I'd recommend CodePen for anything that doesn't require any complicated setup or libraries - just pure HTML, CSS, and JS with optional pre-processors at the top of it. CodeSandbox should be the choice whenever you require any additional setup, UI framework, Node.js, NPM packages, or anything _more complex_.

If you want to use the playground to strengthen your position in the social media or build a personal portfolio, CodePen is a better choice. CodeSandbox is OK, but not as good as its competitor. Posts, collections, exploration page - all these features and a bigger community make CodePen an excellent choice for _social engagement_.

If you use the playground only for embeds on your website or blog, then the complexity case stands. Both editors have great embeds, and the choice should come down to how complex your project is. CodePen, however, might have better _support_ in places, because of its longer presence on the market.

Finally, if you decide to go for a premium plan, CodeSandbox gives you more for less. But, again, if you're doing this for the social engagement, CodePen is worth its price.

# Honorable mentions

Although CodeSandbox and CodePen are the main focus of this comparison, I'd like to mention some other playgrounds that also deserve attention.

## [JS Bin](https://jsbin.com/)

![JS Bin](https://areknawo.com/content/images/2019/12/jsbin.png)JS Bin

_JS Bin_ is a very simple HTML + CSS + JS playground, similar to CodePen's Pens. It allows you to choose from basic pre-processors, link external CDN-based assets, and embed your _bins_ (cause that's what they call them). If you want to code something even quicker than with Pens, JS Bin is a great option.

## [**StackBlitz**](https://stackblitz.com/)

![StackBlitz landing page](https://areknawo.com/content/images/2019/12/stackblitz.png)StackBlitz landing page

Similarly to CodeSandbox, _StackBlitz_ focuses on bringing the VS Code coding experience to the web. Thus, it shares a lot of features with the playground we've already covered. Great editing experience, GitHub repo imports, and quick [Firebase](https://firebase.google.com/) deployments are only some of its advantages. The project is growing quickly, and you might want to check it out.

## [Repl.it](https://repl.it/)

![Repl.it landing page](https://areknawo.com/content/images/2019/12/repl.png)Repl.it landing page

[_Repl.it_](http://repl.it/) can be considered the best of CodeSandbox and CodePen combined. Great editing experience with the help of auto-completion, quick deployments, Git integrations, and vast social & community features make [Repl.it](http://repl.it/) a full-blown _programming platform_.

Comments, challenges, posts - all that is there. But, what's the most impressive about this editor, is the fact that it doesn't limit itself to web technologies, allowing you to play with many _different languages_, like C++, Go, Rust, Python & more!