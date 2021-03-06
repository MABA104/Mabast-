---
title: The Ember Times - Issue No. 79
author: Chris Ng, Jessica Jordan, Kenneth Larsen, Michael Schinis
tags: Newsletter, Ember.js Times, Ember Times, 2019
alias : "blog/2019/01/04-the-ember-times-issue-79.html"
responsive: true
---

Blein Vie Noa, Emberistas! ๐น๐๐

The new year starts off with loads of **new RFCs**! Read more about suggested **deprecations** of **Route render** methods and selected **ApplicationController properties** ๐ธ! We also have a new RFC for a **brand new look** of emberjs.com, **performance improvements** ๐ for the API Docs **search**, a new beta release of **ember-cli-babel** and an advanced testing **exam** for you!

---

## [Website Redesign ๐จ](https://github.com/emberjs/rfcs/pull/425)
The official Ember website is due for a new look and feel. That is why a [new RFC](https://github.com/wifelette/rfcs/blob/master/text/0425-website-redesign.md) proposes a **completely new look** ๐ for emberjs.com. A side effect of not having updated the look and feel of the website for some years is that for people who arenโt involved in the day-to-day of Ember development, itโs **easy to miss just how well the framework has kept up over the years**.

 The redesign aims to **modernize, update and improve all the things on the website** so that the impression given to the general public matches reality.

Thereโs already a good discussion going on in the [RFC comment section](https://github.com/emberjs/rfcs/pull/425), and we would love to hear your thoughts as well.

---

## [Deprecating Route Induced Rendering ๐จ](https://github.com/emberjs/rfcs/pull/418)

Do you remember `Route.render()` and `Route.renderTemplate()`? You might not. In fact, these route methods have been less and less emphasised in the Ember learning story and are not even mentioned in the [Ember Guides](https://guides.emberjs.com/release/) anymore. Although these APIs were useful in the past, nowadays a component-focussed approach allows Ember developers to omit them entirely.

Therefore, a **new RFC** suggests the **deprecation** of `Route#render` and `Route#renderTemplate`. You can read more about the motivation behind it and how to replace these methods in your application in [the original proposal](https://github.com/emberjs/rfcs/blob/ddbf21eaefae946a7e97573fec10334fb104e259/text/0418-deprecate-route-render-methods.md).

Questions? Suggestions? Leave them right in the [comments section of the RFC](https://github.com/emberjs/rfcs/pull/418)!

---

## [Deprecating Router Props on Application Controllers ๐](https://github.com/emberjs/rfcs/pull/421)

With the introduction of [the Router Service](https://www.emberjs.com/api/ember/release/classes/RouterService) it's been easier than ever to check on current app state, e.g. the name of the active route, anywhere in your application. This also means that the current `ApplicationController#currentPath` and `ApplicationController#currentRouteName` API has become obsolete.

A **new RFC** proposes the [deprecation of these abundant properties](https://github.com/emberjs/rfcs/blob/a7ea6898280cd065cb5183d3245cceba3fd2e91b/text/0421-deprecate-application-controller-props.md) in the future. Be sure to [let your thoughts known in the proposal's comments section](https://github.com/emberjs/rfcs/pull/421)!


---

## [API Search Performance ๐](https://twitter.com/mschinis/status/1080923571109724162)

<img class="float-left large transparent padded pad-l0" alt="Algolia search improvements" src="/images/blog/emberjstimes/algolia-search-performance-improvements.png" />

The integration with our search provider, [Algolia](https://www.algolia.com/) that powers both [Ember Guides](https://github.com/ember-learn/guides-app) and [Ember API Docs](https://github.com/ember-learn/ember-api-docs) has now become even more performant!

The work from our friends at Algolia unlocked a performance boost of the API docs search by as high as 285% for some countries in Europe! The map shows data centers where the API docs are currently stored and (on the right) the performance improvement for the top searching countries.


---

## [New Beta Release for ember-cli-babel ๐](https://twitter.com/pzuraq/status/1075856318798344192)

[@pzuraq](https://github.com/pzuraq) recently announced the release of [ember-cli-babel@v7.3.0-beta.1](https://github.com/babel/ember-cli-babel/tree/v7.3.0-beta.1)!

The plugin [ember-cli-babel](https://github.com/babel/ember-cli-babel) uses [Babel](https://github.com/babel) and [babel-preset-env](https://github.com/babel/babel-preset-env) to allow us to use ES6 syntax within our Ember CLI project.

With the 7.3.0 beta release, the `includeExternalHelpers` option is now available. This option controls deduplicating the default Babel helper functions by putting them in a shared module and lowering the payload size.

To read more on the `includeExternalHelpers` check out the [docs](https://github.com/babel/ember-cli-babel/#external-helpers)!

---

## [Improving Testing One Partition at a Time ๐ฐ](https://github.com/emberjs/rfcs/pull/426)

**Ember's testing story** already makes testing incredibly approachable to developers, but what if it could bring even more to the table right from the start? Imagine being able to speed up your test suite with **parallel testing** or running tests in **randomized order** with a simple `ember test` command in your app.

A new [RFC proposes an update to the testing default in Ember apps and addons](https://github.com/emberjs/rfcs/pull/426) by providing [ember-exam](https://github.com/ember-cli/ember-exam) - an Ember addon developers can already use for advanced testing strategies - built into Ember's testing setup.

Be sure to **read the full proposal** and leave your [thoughts in the comments below](https://github.com/emberjs/rfcs/pull/426)!


---

## [Contributors' Corner ๐](https://guides.emberjs.com/release/contributing/repositories/)

<p>This week we'd like to thank <a href="https://github.com/zeppelin" target="gh-user">@zeppelin</a>, <a href="https://github.com/Turbo87" target="gh-user">@Turbo87</a>, <a href="https://github.com/jamesgeorge007" target="gh-user">@jamesgeorge007</a>, <a href="https://github.com/ppcano" target="gh-user">@ppcano</a>, <a href="https://github.com/rwjblue" target="gh-user">@rwjblue</a>, <a href="https://github.com/chrisrng" target="gh-user">@chrisrng</a>, <a href="https://github.com/jessica-jordan" target="gh-user">@jessica-jordan</a>, <a href="https://github.com/mschinis" target="gh-user">@mschinis</a>, <a href="https://github.com/kennethlarsen" target="gh-user">@kennethlarsen</a>, <a href="https://github.com/nummi" target="gh-user">@nummi</a>, <a href="https://github.com/rwwagner90" target="gh-user">@rwwagner90</a> and <a href="https://github.com/mixonic" target="gh-user">@mixonic</a>  for their contributions to Ember and related repositories! ๐</p>

---

## [Got a Question? Ask Readers' Questions! ๐ค](https://docs.google.com/forms/d/e/1FAIpQLScqu7Lw_9cIkRtAiXKitgkAo4xX_pV1pdCfMJgIr6Py1V-9Og/viewform)

<div class="blog-row">
  <img class="float-right small transparent padded" alt="Office Hours Tomster Mascot" title="Readers' Questions" src="/images/tomsters/officehours.png" />

  <p>Wondering about something related to Ember, Ember Data, Glimmer, or addons in the Ember ecosystem, but don't know where to ask? Readersโ Questions are just for you!</p>

<p><strong>Submit your own</strong> short and sweet <strong>question</strong> under <a href="https://bit.ly/ask-ember-core" target="rq">bit.ly/ask-ember-core</a>. And donโt worry, there are no silly questions, we appreciate them all - promise! ๐ค</p>

</div>

---

## [#embertimes](https://emberjs.com/blog/tags/newsletter.html) ๐ฐ

Want to write for the Ember Times? Have a suggestion for next week's issue? Join us at [#support-ember-times](https://discordapp.com/channels/480462759797063690/485450546887786506) on the [Ember Community Discord](https://discordapp.com/invite/zT3asNS) or ping us [@embertimes](https://twitter.com/embertimes) on Twitter.

Keep on top of what's been going on in Emberland this week by subscribing to our [e-mail newsletter](https://the-emberjs-times.ongoodbits.com/)! You can also find our posts on the [Ember blog](https://emberjs.com/blog/tags/newsletter.html).

---


That's another wrap! โจ

Be kind,

Chris Ng, Jessica Jordan, Kenneth Larsen, Michael Schinis and the Learning Team
