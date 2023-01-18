# Networking Considerations

### Networking Designs
In the lead-up to figuring out a solution, leading to this new direction for [[Webizen 3.0]], i was struggling to figure out how to get the networking solution done. 

This paper was written as a consquence of trying to figure out that problem.

The Short Answer is, that the plan for Low-Level Networking is to use [Tailscale](https://github.com/tailscale/tailscale) and [Headscale](https://github.com/juanfont/headscale) then looking to update [Caddy](https://github.com/caddyserver/caddy) which is [already set-up to support Tailscale](https://tailscale.com/blog/caddy/).  

Whereas, the information networking methodology is actually far more complex...

## OVERVIEW

The Webizen Platform is intended to be a force for good, as is an overriding objective of significance.  The platform itself; is intended to support an information management system that works in a way that is different to other known ‘operating systems’, application environments and consequently thereafter - information management solutions.  These works are complex, and consider various ‘spheres’ from the technical (infosphere) to the socio-sphere, economic, legal, biosphere, etc. The platform has a focus on producing ecosystem solutions to usefully employ AI.

### Background Notes;

1.  The works done by me, with others, in these areas dates back to the 1995-6 or so; although those were very early days, and a great deal more was achieved from 2000 onwards.  Some of the old diagrams continue to present models, that remain similar; whilst some of the problems that were experienced even back then, still remain & in some ways have become far worse or minimally described - different, overtime.  
    
2.  By 2010 works had started on employing HTTP ‘Semantic Web’ tooling; which in-turn led to a significant involvement in the creation of new ‘web standards communities’ which led to new standards, of vast significance to humanity at large; given how they’ve been implemented.  Standards work is a different job, to producing software / applications that make use of the tools produced & made available (royalty free ‘patent pool protected’ standards, etc); to produce particular products, and as time goes on requirements shift.
    
3.  A Major constituency of the purposeful efforts has been to support human rights related ‘technological infrastructure’ apparatus.  A design focus, has been to consider the needs of the poor, the vulnerable and those in need of accessible & appropriate support for lawful considerations & available legal recourse / remedy (ie: natural justice); which is now demonstrably shown to have been an unusual focus, given what has been supported; and what continues to be in an area of distressing problems, that have not been resolved. 
    
4. Whilst the modelling has direct applications for incorporate entity infrastructure (ie: corporate, government, education; in all the many areas); individuals in their private capacities needs to be provided ‘digital agency’ in-order to support anything else well; these considerations are discussed via the lens of ‘values’ and in particular ‘human rights’,

5. Service to support ‘human rights’ are presently expensive (at least $120 AUD / PA, per entity group (ie: individual or family);  including but not limited to,
	a.  The Rental Costs for a Domain Name
    b. The Service Costs for an online (“cloud”) server (hosting / vps, etc.) that provides support for ‘fixed IPs’ (HTTPS support)
    
6. The ability to support ‘home “read/write” applications that employ HTTP services (which is often not supported by residential internet connections); which in-turn means, that some sort of VPN like functionality is required.  
      
    NOTE: online services are subject to ‘choice of law’ terms, which are often not in the same jurisdiction as the intended beneficiary of that apparatus (indeed, they’re often not even in the same country).  

7.  Technically; ‘Semantic Web’ uses HTTP URis. Whilst other non-http based protocols can be employed, there is still a requirement to ensure support for HTTP(s) & DNS (ie; domain name, email, etc) services.  There is also a lack of support for IPv6 in many areas, alongside other legacy issues linked to ICANN (the domain name business); Now therefore, there are complex issues that are emerging as a consequence of ‘web3’ (DLTs) solutions that are not the same as the Web (world-wide-web / www); or other protocols that operate on internet.  
      
    At a social level; the problem becomes the misuse of the concept of ‘identity’ in how it is applied to the use of tooling and the impact that has upon societies.  
      
    At a commercial level; the use of the term ‘identity’ is linked with commercial benefits should any one ‘thing’ (company, blockchain, etc.) control human entities, that is often very difficult to ‘stop using’ - a simple example, would be the dependencies upon public free email addresses provided by large organisations such as Microsoft (hotmail), Google (gmail) and Apple (iCloud) - although; even simply with respect to that one ‘identifier’, the semantic ‘stickiness’ also has implications with respect to accounts provided by internet providers, universities and employers.  Whilst there are MANY examples, the simple one of an ‘email address’, does in-turn have an array of dependency implications across many areas.  
      
    ‘Semantic Web’ refers to an ecosystem of parts principally developed via the W3C; which create the foundational requirements for artificial intelligence services through various tools that define how information is both structured and then able to be employed by systems that have been produced to use ‘semantic web’ tooling.  In-effect, its like Internet Protocol; for electronic (structured) information and information processing related services, which then in-turn powers ‘AI’. The designs required; need to bring the human agent, equitably (and responsibly) into the equations, which is able to be brought about using an ecosystem of tools; that in-turn have dependencies upon the use of HTTP ‘server related’ services. 


## Deliberations: Some recent architectural work and linked considerations.

In a 2017 presentation / talk on [“The End of Cloud Computing”](https://a16z.com/2019/11/15/the-end-of-cloud-computing-2/) General Partner of Andreessen Horowitz Peter Levine explains how cloud technology is changing for an edge cloud model.  

<iframe width="560" height="315" src="https://www.youtube.com/embed/4QTAtFaIiyc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Put simply, Lavine presents the case illustrating how the mass of (IoT) devices ‘at the edge’ requires ‘edge processing’; or in other words, that the computational requirements for devices within ‘personal area networks’ cannot be supported by (international) ‘cloud computing’ capabilities alone.  Reviewing this presentation again recently, reminded me of the physics (in-effect) involved in effectively delivering modern capabilities - even if the moral considerations are not enough.  This ‘battle’ between ‘mainframe’ like systems, and personal computing - is a very old trend.  

I have made a somewhat brief ‘Timeline Exhibit’ of various clips relating in particular to Steve Jobs & Tim Berners-Lee which can be found via the link below.

The creation, production & commercialisation of (cyber) infrastructure - cannot be done quickly enough; yet clearly, the historical / ‘legacy’ business models bound to WWW focused internet services - where global silos are the primary operators / definers of our means for advancement; is indeed problematic, and in-turn also - there are various barriers to creating solutions that can support inter-juristictionality, centred upon the needs of natural persons; as to thereby, uplift any other capacities human beings have in our societies, socio-economically, creatively & otherwise.

These major silos - are in-effect, highly centralised globally as are many ‘DLTs’ (ie: blockchains) although the characteristics are different.  As such, whilst there is a great deal of concern about ‘splinter-net’ or a world of many separate internets - this is in-effect, a difficult puzzle.  From a user-perspective, there’s already ‘separate internets’; such as Microsoft, Apple, Google & facebook; with others in other regions (ie: Asia, etc).   So with that being said…

I find myself looking into VPN technologies as a means to support - in-effect - human agency.  One of the examples I have found is a SDN Networking technology called WireGuard which is then provided a services layer to support private networks via technologies such as TailScale, which is in-turn being supported by other open-source projects such as headscale.  What it does is create a privately addressable network that supports HTTP, TLS, DNS (ETC) enabling private networking of ‘read/write’ (distributed - semantic web based - services); alongside ‘exit nodes’ that provide an ability for a nominated service / server - to provide public-internet connectivity with the rest of the network; that is in-turn connected both, to ‘regular internet’ as well as the ‘private network’ that is set-up using these technologies.  More information about how this particular solution works can be found [https://tailscale.com/](https://tailscale.com/) (inc. blog, etc.). 

Part of what’s also occurring (note headscale, as noted above); is that there’s user-authentication using OIDC; and in-turn also, TLS certificates being issued to devices.  Whilst neither of these solutions appear to support ‘Web-ID’ ecosystem components (ie: SubjectAltName: FOAF (or RDF) URI); it does not appear to be a massive problem to add it; and in-turn, the opportunity becomes, packaging these tools (libraries / services) with either an updated ‘RWW (read-write-web)’ solution or indeed also, the more modern (yet different) solid related variants - or some future harmonisation of both; as a consequence of building and deploying solutions, that ‘make sense’. 

## CONSIDERATIONS: Leading to a Hypothesis

RWW servers were originally designed to employ RDF, LDP WebID-TLS as an authentication instrument; and through that, the server was then able to be extended via various service layers (SPARQL, LDN, etc.).  There are old (webizen related) libraries that exist, but they’ve not been updated.  One example in particular, GOLD (Go Linked Data (or RWW) server) is written in GoLang (“Go”), as are the software libraries for Headscale / Tailscale.  

So, what if there was an integration done to produce ‘client apps’ (nodes) that support both the Private Networking topology with a bundled ‘RWW server’; alongside, a ‘server based’ version (“exit Node” / public gateway / designed for data-center related deployments); that may in-turn also provide support for provisioning & managing a customers domain name; whilst also providing an WebID-OIDC based IdP, that is in-turn used to deploy the WebID-TLS certs on client devices, that via WebID-TLS provides transparent authentication, via the TLS certificate WebID. 

This approach, appears to end-up being closer to the original ‘rww’ works; than the newer’ works (to-date); noting, that the older RWW ‘apps’ (simple HTML5) were very simple to create by comparison to the newer ones(generally NodeJS / server based apps); that are in-fact far more complicated, as are the ‘access control’ issues.  Whilst the ‘decentralisation’ objective is good; the threat becomes, aggregating all of a person's life into a singular container that ends-up being exploited by bad actors; perhaps without any means to know about what might have occurred and/or been deleted or modified.  

## ‘Home as a platform’ vs. ‘gov as a platform’.

Home is where the heart is, but what will AI say, about how government money influences what occurs should people find themselves in a situation where they’ve got some very serious problems at home; what is it, do you think, AI will be able to demonstrate - what they’re priorities have actually been, as demonstrated by the outcomes.  Is the fear of #RealityCheckTech - undermining our capacity for peace?

Much of these works over, particularly over the past 12 years or so; has been undertaken in very difficult circumstances, with the express intent to ensure natural persons (human beings in their private capacity) were provided the technological tools required, to support their relationship with law & therefore, peace.  However, this has not been supported by the government, who has consequently funded the costs of significant harms and consequential enquiries and related costs.  The program known as ‘robodebt’ is a good example of the nature of these decisions; whereby, if people had of been supported to be able to store their own electronic evidence / legal records of importance; then, providing machine-readable payslips would have been easily performed and/or compelled to have been performed via lawful means.

There is insufficient evidence to reasonably support any claim that Government will of its own volition, provide the cyber-infrastructure requirements needed by citizens, to protect their rights unto law and in-turn, act to support both our system of government and our means to protect our society from the harmful consequences of those engaged in organised activities causing serious injury to others; by ensuring, circumstances of a nature that should reasonably lead to a complaint being made in a court of law, are provided the supports needed to demonstrate governmental commitments to the various instruments that exist; whether it be UN instruments, including but not limited to the UDHR, or the principles set-forth in the Charter of the Commonwealth or indeed the specific statements made by various state and federal laws / legislation, conventions and legal precedents.  Put simply, the importance of useful employment of law / rule of law and in-turn its very important role with respect to peace and human rights; has not been demonstrated to have been provided the respect or support, needed, to protect the most vulnerable in our society, which is not about any discriminatory factors alone; rather, that the complex consequences of not providing an opportunity for alternative ‘business systems’ to emerge inter-domestically, will not stop the consequences of what will otherwise occur as Artificial Intelligence grows in its capacities and influences, via globally centralised platforms; or via alternative ecosystems.

## Webizen Networks - by WebCivics (& Trust Factory)

Webizen is a project that seeks to produce a new class of computing environment that incorporates many complex concepts that are not well understood by the vast majority; particularly, the details. 

Nonetheless - The broad-strokes of it, is that its a sort of ‘information management fabric’ that i’ve been working on for a very long time; and, now decades later, there’s a bunch of work done by various other people around the world, many luminaries involved, whose collective efforts; enable the creation of an ecosystem, that works to address various - very significant problems; social, economic, cyber, (inc. AI), etc.

The hypothesis (as I've put it); of employing some sort of networking solution like the one mentioned, appears to reduce the effective entry-level cost significantly.  I think, its important to stipulate & structure the organisational approach (reflected in-turn by the technology topology) to support ‘common jurisdictional presence’ for legal entities; which in-turn means, that ‘by default’, users would ‘sign-up’ to a webizen networking / Semantic (AI) SDN service that has contractual arrangements within their jurisdiction.

These systems also maintain some level of ‘controls’ via the end-node interfaces and the capabilities built there.  In a worst-case scenario where a bad-actor needs to be ‘shut-down’ that could be done at the IdP; equally, an array of other capabilities can be provided as a distributed processing capability, providing HTTP services whilst at a lower-cost than is otherwise able to occur, through the use of existing VPS solutions alone.  This business model, requires support via a particular form of commercial (for purpose) approach; but, is aimed at providing mechanisms / methodologies, to support a differentiation between the capabilities needed to defend our societies from the threats of crime internationally; vs. domestic / local approaches, and in-turn also (governance) responsibilities and other aspects relating to the ‘right to self determination’ (human rights / democracy / prevention/protection from foreign interference, etc.) & access to justice. 

So, if this were done in a way; that is consistent with the various ‘human rights’ related considerations, which in-turn relate to licensing and other mechanisms to support dignity and address ‘digital slavery’ issues; whilst maintaining (indeed enhancing) support for the creation of software for the good of humanity; there are centralisation related implications, unlike ‘web 2.0’ or “#Web3”; and provide a capacity to produce electronic governance frameworks, to support cooperative, Collaborative and supportive socio-economic ecosystems, Inter-juristictionally / internationally; noting, these systems, do not prevent ‘old internet’ from continuing to function, it just provides a different environment for different kinds of apps / computing platforms / work & AiTech environments; that seeks, to mediate operational tasks, in a way that accelerates our capacity to improve productivity and radically extend our support for a regenerative and rejuvenative evolutionary paradigm shift, as a consequence of good designs for the use of ICT Tools. 

 Yet, this is an R&D process; which is expected to evolve overtime and will be particularly vulnerable at the early stages of any ‘commercialisation’ (including software production); via well funded adversaries. 

## Design Considerations - as an initial ‘options analysis’ derivative.

IF, this path is investigated and/or further developed; then considerations are as follows,

### User Experience

1.  User goes to webizen.au (for example) and sets-up an account.
    
2.  Once the account is setup (with or without their own domain, etc.) then they can download ‘client software’ which is basically a ‘vpn’ like thing that has a RWW ‘social-web /  webizen server’ baked into it; which then operates in a federated manner with other devices in their ‘private network’.
    
3.  User then creates or downloads apps that depend upon these services existing; whereby the app is simply ‘client side’ pulling the data from the network; and using local machine resources to perform various tasks. (there are various libraries for Go app development that support interfaces for media processing, cuda, tensor, etc.). 
    
4.  The user then downloads the clients for other devices; and the ‘information environment’ works in a federated manner.  This provides an opportunity to assign ‘capabilities’ of different devices in the users network, and distribute tasks to different agents (servers) programmably.
    

### Notes about ‘solid’ vs. RWW vs. ‘Webizen’

As noted in related documentation, the term ‘webizen’ was used by the ‘original ‘RWW’ team; and whilst honouring their efforts is part of the moral goals of the project; there are also alot of changes being made.

-   It's not seemingly a topology that is ‘the same’ as solid: there are other factors / elements of the broader ‘webizen’ design that are also different, so this isn’t necessarily a problem, noting, solid is also a ‘work in progress’ and their specifications may well change based upon what Tim Berners-lee (or other influencers involved) believe is the most appropriate approach, as does develop overtime.  
      
-   There is possibility of providing, what is in-effect, ‘transparent’ authentication at the ‘device’ or ‘user-account’ level; via the TLS certificate (WebID-TLS / WebID-RSA, etc) to personalise the session, which is in-turn authenticated against a user when they set-up the network ‘node’.  
      
-   An ability to support some sort of log-in/log-out (WebID-OIDC based) on shared computers is needed.  There are also considerations to make about others using someone else's device (ie: children, or someone else - who may not be behaving in a ‘friendly’ manner).
    
-   2nd factor AUTH could be supported via various devices in a network (ie: a smartphone) by assigning that device a role to perform that task.  This and many other ‘features’ / workflows; would ideally be relatively simple to create (ie: via web-assets rather than continual upgrades to the underlying compiled runtime) as often as possible.  
      
-   Another implication is that, due to the ‘data storage structure’, disconnection from the network doesn’t result in a user loosing their data; which is one of many positive qualities of this approach.  
      
-   The future ‘webizen’ platform - will require a great deal more work & capabilities to deliver the sorts of capabilities that is sought to be brought about; whether or not ‘go’ is right for the client in the long-term, is yet to be known.  There are ‘bindings’ for other languages; but overall, there’s a need to create a platform that can support the development of the broader ‘webizen’ project, including but not limited to the delivery of initial that are very much focused on providing a ‘solid’ or ‘rww’ like, environment, that can be easily employed by persons working from home or wherever they are; to collaboratively do work through ‘web apps’ that are cheaply employable.   
      
    Without forming some sort of decentralised foundation for how people are able to work with one another; the outcome of being able to decentralise and support the purpose of these works, has never before actually been delivered.  In-part, this is a commercial issue that’s hard to address once investment has gone into whatever the ‘proof of concept’ body of work is; and thereby, socialised to other persons whose focus is most often about how to make the most out of it all.  
      
-   A Loosely coupled approach; could also provide support for other groups to produce similar solutions using different protocols, or indeed also, the ability for future clients; to support an array of different protocols - a bit like plugins or extensions i guess…  This would in-turn require a specification defining what is required to support specific functionality in relation to use cases.
    
-   Note also; there are various ‘packages’ such as ‘nextcloud’ and its office-app functionality, alongside various other ‘web-apps’ that can be run relatively easily, on a high-powered laptop or desktop like device (basically - on consumer equipment); but the hosting costs / set-up processes, have historically been prohibitive.   
      
    Whilst further integration opportunities are very interesting, there’s also a meaningful opportunity to provide near-immediate support for users to get these sorts of platforms working at home, at nominal cost, for private groups; which is envisaged to significantly uplift innovation & productivity.  


# GOALS

1.  To investigate & identify if there’s any interest in this approach; and if there’s any significant flaws associated with going down this path; should we pass this precondition; then,
    
2.  Funding is desirable and the organisation should be set-up to support development & Go To Market (“GTM”) works in addition to the works required to develop an international ‘Community’.
    
3.  A Software Development project to integrate the networking stack with the ‘RWW / Solid’ (more RWW than solid, imo) tooling; to produce both installable clients for consumer devices; as well as a ‘host platform’, that is designed to support the functionality only able to be supported via data centre hosting.  Additional software development projects would include the ‘apps’ (social, modifications to existing RWW(/early solid) apps & the work project).


