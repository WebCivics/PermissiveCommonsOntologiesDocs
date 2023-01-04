The objective of this project is to create a runtime environment for the use of RWW / solid like applications that are built using HTML5 (HTML/CSS/JS) on personal computers.  The focus of the first stage is to deliver an ecosystem that operates on laptop & desktop machines, with the support of a low-cost server (or server-side service) that provides networking support and related features built upon the tailscale / headscale networking packages.

The use of obsidian is experimental and these product / functionality specifications are likely to be updated overtime. 

**HIGH LEVEL OBJECTIVES**

The high-level objective, is to create some initial open-source software packages, that provide an ability for users to either download a server-runtime that can be set-up on a VPS to support private networking support with 'client' applications that are installable on Windows & OSX in particular (also linux, but not the priority); or, that the user is able to use the 'webizen' / webcivics install that is set-up to support users.

Users then download the 'client' apps, and set them up on their local machine (ie: OSX/Windows/linux) which in-turn provides them a folder they can drop HTML5 apps written for that 'webizen server' that uses WebID-TLS (from the local host rww server) and optionally also WebID-OIDC (via the remote host / 'control server').  

The client apps are able to be written using basic HTML5 tools; and the server provides the basic 'hooks' needed to perform various functions  (described later).

The instances use semantic web technologies to create decentralised 'social' application environments.  ACLs are managed by the user, via WebID related ACLs; which are in-turn built upon the namespace (entity centric).  Local apps do not provide any data to 3rd party systems unless expressly requested to do so.  This mechanism is sought to be achieved using 'verifiable credentials' (or openbadges) related methods (alongside WAC).   The more advanced aspects of how these systems should be implemented requires an operating environment that has some apps functioning on it, in-order to further develop the semantic logic processes. 

In-order to achieve that objective quickly; a method has been identified to use (and update accordingly) existing go libraries - as to achieve the objective of building a basic environment that is able to be used by people who are not necessarily software engineers (ie: might have various types of skills that are important for progress); and, until there is something that operates in a manner that exemplifies how these systems are intending to create a different sort of ecosystem, its hard to explain. 

NOTE:  One of the first projects sought to be developed (after the basics are done) is a 'work platform' or app / ecosystem environment. The purpose of this 'app' / ecosystem environment; is to support decentralised development of projects, including the means to attribute resource value (project costs) which may in-turn articulate to future income (roi / compensation); using dual-licensing and other complex methods, as to support the competing interests of seeking to end-up providing open and freely available software for the betterment of mankind; whilst ensuring the method employed to do so, does not breach human rights / engender 'digital slavery'.  This project is about getting long-term works to a next milestone; and one / if that is achieved, then there is still a long way to go.

OUTCOME
The outcomes of this project seek to achieve the following objectives;
1. Users should be able to 'sign-up' online; and,
	a. create an WebID-OIDC Address; and,
	b. connect a domainname (or are alternatively provided one)
	c. be provided a basic webspace (html5) that can use local graph resources.
3. Install 'clients' that create a networking environment that supports HTTPS & WebID-TLS using that domainname.
4. Create and/or download/install 'webizen v1 apps' (rww/solid based) onto their 'home' webizen server/client.

Once these objectives are achieved, it is considered that users will be able to 'push' resources (different acls, etc.) to different nodes (ie: from their local machine, to the 'host' that's supporting some sort of 'public webpage', blog, etc.); and that this is achieved via the 'apps' that are created on top of this 'webizen v1 platform' stack.

Development Tools Summary

Primary Codebase
In-order to develop something that works quickly, it has been found that a number of  critical functionality requirements is able to be supported by existing GoLang projects.  Alternatives have not been found using nodejs libraries or otherwise.

These libraries include; but are not limited to,

Client / Server Side Packages

Headscale (https://github.com/juanfont/headscale) 
Headscale is an opensource implementation of the TailScale Control Server.  It provides an ability for users to set-up an account via OIDC (openID connect) and initiate a private network based upon the tailscale network technologies; that can then be routed both privately and publically, using an 'exit node'

Tailscale (https://github.com/tailscale/tailscale) 
Tailscale provides both client and server packages for networking.  It provides a private network that supports TLS & IPv4/IPv6; enabling routing through firewalls (like a vpn).  It is controlled by a 'control server', headscale is an open-source project working to build one.

Caddy Server (https://github.com/caddyserver/caddy)
Caddy Server is an extensible web-server written in Go.  It is integrated with Tailscale.

RWW Server
In the project now commonly known as solid, however earlier known as RWW (or crosscloud) there was a server implementation in GOlang. 
GOLD ( https://github.com/linkeddata/gold )

Another library (unknown level of development) called helix (https://github.com/deiu/helix) also exists. 

**Other libraries**
There's an array of other libraries that may be usefully employed and/or considered from an architectual point of view for future releases.  This does include; in-particular,
- Graph Database libraries (NB: https://github.com/cayleygraph/cayley)
- Credentials / Verifiable Credentials (nb: https://pkg.go.dev/github.com/hyperledger/aries-framework-go/pkg/doc/verifiable )

This is a non-exhaustive list and more information / research about the options is being compiled into this documentation environment.