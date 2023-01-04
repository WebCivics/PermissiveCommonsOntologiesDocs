---
id: 610
title: 'Solutions to FakeNews: Linked-Data, Ontologies and Verifiable Claims'
date: '2018-10-04T10:21:31+10:00'
author: ubiquitous
layout: page
guid: 'https://www.webizen.net.au/?page_id=610'
inline_featured_image:
    - '0'
---
```html
[**Linked-Data**](https://www.webizen.net.au/what-is-linked-data/)<span style="font-weight: 400;"> is a technology that produces machine and human readable information that is embedded in webpages. Linked-Data powers many of the online experiences we use today, with a vast array of the web made available in these machine-readable formats. The scope of linked-data use, even within the public sphere, is rather [enormous](http://lod-cloud.net/)</span><span style="font-weight: 400;">.</span>

<span style="font-weight: 400;">Right now, most websites are using ‘linked data’ to ensure their news is being presented correctly on [Facebook](http://ogp.me/#)</span><span style="font-weight: 400;"> and via search, which is primarily supported via </span>[<span style="font-weight: 400;">Schema.org</span>](https://schema.org/docs/about.html) <span style="font-weight: 400;">.</span>

**The first problem is:**<span style="font-weight: 400;"> that these ontologies do not support concepts such as [genres](https://en.wikipedia.org/wiki/Genre)</span><span style="font-weight: 400;">. This means in-turn that rather than ‘news’ becoming [classified](https://en.wikipedia.org/wiki/List_of_genres)</span><span style="font-weight: 400;">, as it would in any ordinary library or newspaper, the way in which ‘news’ is presented in a machine-readable format is particularly narrow and without (machine readable) context. </span>

<span style="font-weight: 400;">This means, in-turn, that the ability for content publishers to self-identify whether their article is an ‘advertorial’, ‘factual’, ‘satire’, ‘entertainment’ or other form of creative work – is not currently available in a machine-readable context. </span>

<span style="font-weight: 400;">This is kind of similar to the lack of ‘emotions’ provided by ‘social network silos’</span><span style="font-weight: 400;"> to understand ‘sentiment analysis’ (EG: research links [1](http://people.sabanciuniv.edu/berrin/share/LDA/Stanford-NLP-Course-termproject-ssoriajr-kanej.pdf) and [2](https://blogs.msdn.microsoft.com/jennifer/2016/06/28/sentiment-analysis-on-social-network-data-twitter-facebook-etc/)) </span><span style="font-weight: 400;"> through semantic tooling that offer means to profile environments</span><span style="font-weight: 400;"> and offer tooling for organisations. Whilst Facebook offers the means to moderate particular words for its pages product</span><span style="font-weight: 400;"> this functionality is not currently available to humans (account holders). </span>

<span style="font-weight: 400;">The mixture of a lack of available markup language for classifying posts, alongside the technical capabilities available to</span>*<span style="font-weight: 400;"> ‘persona ficta’</span>*<span style="font-weight: 400;"> in a manner that is not similarly available to Humans, contributes towards the lack of ‘human centric’ functionality these platforms currently exhibit. </span>

**Bad Actors and Fact-Checking**

<span style="font-weight: 400;">In dealing with </span>**the second problem** <span style="font-weight: 400;">(In association to the use of Linked-Data), the means in which to verify claims is available through the application of ‘credentials’</span><span style="font-weight: 400;"> or [Verifiable Claims](https://www.webizen.net.au/about/knowledge-banking-a-technical-architecture-summary/what-are-credentials/)</span><span style="font-weight: 400;"> which in-turn relates to the Open Badges Spec</span><span style="font-weight: 400;">.</span>

<span style="font-weight: 400;">These solutions allow an actor to gain verification from 3rd parties to provide their audience greater confidence that the claims represented by their articles. Whether it is the means to “fact check” words, ensure images have not been ‘photoshopped</span><span style="font-weight: 400;">’ or other ‘verification tasks’, one or more reputable sources could use verifiable claims to in-turn support end-user (reader / human) to gain confidence in what has been published. Pragmatically, this can either be done locally or via the web through 3rd parties through the use of Linked-Data. For more information, get involved in W3C</span><span style="font-weight: 400;">, you’ll find almost every significant organisation involved with Web Technology debating how to build standard to define the web we want</span><span style="font-weight: 400;">.</span>

<span style="font-weight: 400;">  
</span><span style="font-weight: 400;">General (re: Linked Data)</span>

<span style="font-weight: 400;">If you would like to review the machine-readable markup embedded in the web you enjoy today, one of the means to do so is via the [Openlink Data Sniffer](http://osds.openlinksw.com/)</span><span style="font-weight: 400;"> An innovative concept for representing information was produced by Ted Nelson</span><span style="font-weight: 400;"> via his Xanadu Concept</span>

<iframe allowfullscreen="allowfullscreen" frameborder="0" height="315" loading="lazy" src="https://www.youtube.com/embed/En_2T7KH6RA?rel=0" width="560"></iframe>

<span style="font-weight: 400;">Advancements in Computing Technology may make it difficult to trust media-sources</span><span style="font-weight: 400;"> in an environment that seemingly has difficulty understanding the human-centric foundations to our world; and, where the issues highlighted by many, including Eben Moglen</span><span style="font-weight: 400;">, continue to grow. Regardless of the technical means we have to analyse content (ie: [redlink demo](https://my.redlink.io/#/apps/DEMO/playground)) </span><span style="font-weight: 400;">, it will always be important that we consider virtues such as [kindness](https://lists.w3.org/Archives/Public/public-schemaorg/2016Nov/0063.html)</span><span style="font-weight: 400;">; and, it is important that those who represent us, in seeking solutions for [vulnerable people](https://lists.w3.org/Archives/Public/public-credentials/2016Feb/0069.html) us, put these sorts of issues</span><span style="font-weight: 400;"> on the agenda in which “fake news” has become yet another example (or symptom) of a much broader problem (imho).</span>

<iframe allowfullscreen="allowfullscreen" frameborder="0" height="315" loading="lazy" src="https://www.youtube.com/embed/aiFIu_z4dM8?rel=0" width="560"></iframe>

<span style="font-weight: 400;">A simple (additional) example of how a ‘graph database’ works as illustrated works such as this DbPedia related example (see: [visualdataweb.org](http://www.visualdataweb.org/) original example broken).</span><span style="font-weight: 400;"> The production of “web 3.0”</span><span style="font-weight: 400;"> is remarkably different (see: [startups to smartups](http://jeffsayre.com/2010/09/13/web-3-0-powering-startups-to-become-smartups/)) to former versions due to the volume of pre-existing web-users. Whilst studies have shown that humans are not really that different</span><span style="font-weight: 400;">, the challenge becomes how to fund the development costs of works that are not commercially focused (ie: in the interests of </span>*<span style="font-weight: 400;">‘persona ficta’</span>*<span style="font-weight: 400;">) in the short-term, and to challenge issues such as ‘fake news’ or indeed also even, how to find a ‘Toilets’</span><span style="font-weight: 400;">. </span>

<figure aria-describedby="caption-attachment-613" class="wp-caption aligncenter" id="attachment_613" style="width: 525px">[![](https://www.webizen.net.au/wp-content/uploads/2018/10/Screen-Shot-2016-08-30-at-6.46.45-PM-1024x705.png)](https://www.webizen.net.au/about/applied-theory-applications-for-a-human-centric-web/solutions-to-fakenews-linked-data-ontologies-and-verifiable-claims/screen-shot-2016-08-30-at-6-46-45-pm/)<figcaption class="wp-caption-text" id="caption-attachment-613">Searching for a public Toilet (google search, 30 August 2016)</figcaption></figure><span style="font-weight: 400;">As ‘human centric’ needs continue to be unsupported via the web or indeed also, the emerging [intelligent assistants](https://en.wikipedia.org/wiki/Intelligent_personal_assistant)</span><span style="font-weight: 400;"> working upon the same datasets; the problem technologists have broadly produced becomes that of a world produced for things that ‘sell’, without support for things we value. Whether it be support for how to help vulnerable people, receipts that don’t fade (ie: not thermal, but rather machine-readable), civic services, the means to use data to uphold ‘rule of law’, vote and participate in civics or the array of other examples in which we have the technology, but not the accessible application in which to apply the use of our technology to social/human needs. </span>

<span style="font-weight: 400;">Indeed the works we produce and contribute on the web are for the most-part provided not simply freely, but at our own cost. The things that are ‘human’ are less important and indeed, poorly supported. </span>

<span style="font-weight: 400;">This is the bigger issue. We need to define means to distil the concept of ‘dignity’ on the web. Apps such as Facebook often have GPS history from our phones; does that mean the world should use that data to identify who broke into a house? If it is said you broke a speed limit in your vehicle when the GPS records show you were somewhere else, how should that help you? </span>

note; this article is based upon an earlier post re: [solutions to fake news.](https://docs.google.com/document/d/1OPghC4ra6QLhaHhW8QvPJRMKGEXT7KaZtG_7s5-UQrw/edit#)

```
