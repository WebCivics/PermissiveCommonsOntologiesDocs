The concept of Decentralised IDentifiers was first raised on the [W3C WebPayments Mailing list in 2014 by Manu Sporny](https://lists.w3.org/Archives/Public/public-webpayments/2014May/0033.html) (and Dave Longley who originally registered the [URI Scheme with IANA](https://web.archive.org/web/20181225121742/https://www.iana.org/assignments/uri-schemes/prov/did)

(whilst i'm noted - often the context of these calls was that they were held in the early hours of the morning (ie: 3AM Sydney/AU Time)).

Whilst the works have developed significantly, there are some particular use-cases relating to a concept called [Self Sovereign Identity](http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html) that has been the primary focus of these works.

From my point of view, the useful purpose of DIDs in particular (not withstanding others); was to support the permissive commons requirements in a standardised sort of way.  

Whilst i am supportive of the use of a method to support non-http uris for resources that make use of linked data / RDF and related ecosystem technologies, i am presently unsure whether and/or how well, the DID specifications now provide a fit-for-purpose solution, and there's been some fairly emotionally explosive history, relating to the history of this tech.

### Top Level Resources
- IANA: https://www.iana.org/assignments/uri-schemes/prov/did 
- IETF https://datatracker.ietf.org/doc/html/draft-mayrhofer-did-dns-05
- W3C
	- Methods Registry: HTML: https://w3c.github.io/did-spec-registries/#did-methods 
	- Methods Registry: GitHub: https://github.com/w3c/did-spec-registries/
	- W3C Working Group: https://www.w3.org/2019/did-wg/
	- W3C Credentials CG: https://github.com/w3c-ccg/community/blob/main/work_items.md 
- DIF:  https://identity.foundation/ 
- ID2020: https://id2020.org/
- Trust Over IP: https://trustoverip.org/
- Mastercard 
- GS1: 
- Microsoft: https://www.microsoft.com/en-us/security/business/solutions/decentralized-identity

and many others...  (note; [DID methods registry](https://github.com/w3c/did-spec-registries/tree/main/methods))

#### Discomfort

Perhaps part of my problem could be based upon upset relating to my personal experiences, and that the technological output is indeed fit for purpose; yet the problems that i am concerned about stem from issues that do not relate to the specifications.  This is something that i will work through to figure out more formally.  I note, that the commercialisation of DIDs via Vaccine Passports - horrified me.  I felt personally let down, and deeply concerned and upset about the implications.

### Bit of History.
I was involved with the beginnings of this work, whereby I particularly supported Manu Spory as the Brains Trust for this and related works.  The earlier history involved works on [Web Payments Standards](https://www.w3.org/community/webpayments/) which led to [Credentials CG](https://www.w3.org/community/credentials/2014/08/06/call-for-participation-in-credentials-community-group/) which was originally focused on Verifiable Claims and improving the [[OpenBadges]] standards; which overtime led to DIDs.

Prior to the creation of Decentralised Identifiers, previous projects included WebDHT and HTTPA.  The hope was that DIDs were going to be the solution for providing permissive commons; however in more recent years, the works appear to have taken a turn towards being defined by many as 'Decentralised IDentity' which has some percieved problems, that i do not like or support; noting, that the underlying issues relating to these percieved problems are complex, and that i very much support the ability to have Verifiable Claims and Verifiable Credentials.

DIDs are also very closely related to various #Web3 and #Web5 works, that aren't actually about the use of the World Wide Web very much at all - whilst noting again, the complexities involved.  Perhaps most of all; an ecosystem using [[VerifiableCredentials]]  and [[DIDs]] emerged and had a significant global role in the global promotion, that at times resulted in enforced requirements for people to be delegated 'Vaccine Passports' which appears to have been directly tied to newer members involved in the production of these technologies.  

This had the effect of breaching what i considered to have been a previously considered problem (at the time when works were seeking to advance [[VerifiableCredentials]] to become a chartered W3C Activity ) that i thought was agreed, would not be employed as a 'go to market' usecase.

<iframe width="100%" height="300" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/992760121&color=%23ff5500&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true"></iframe><div style="font-size: 10px; color: #cccccc;line-break: anywhere;word-break: normal;overflow: hidden;white-space: nowrap;text-overflow: ellipsis; font-family: Interstate,Lucida Grande,Lucida Sans Unicode,Lucida Sans,Garuda,Verdana,Tahoma,sans-serif;font-weight: 100;"><a href="https://soundcloud.com/ubiquitous-au" title="Timothy Charles Holborn" target="_blank" style="color: #cccccc; text-decoration: none;">Timothy Charles Holborn</a> · <a href="https://soundcloud.com/ubiquitous-au/credentialscgtelecon2015-06-02medical" title="CredentialsCGTelecon2015 - 06 - 02Medical" target="_blank" style="color: #cccccc; text-decoration: none;">CredentialsCGTelecon2015 - 06 - 02Medical</a></div>

## External Descriptions of DID Technology


### Wikipedia: What are DIDs?

**Decentralized identifiers** (DIDs) are a type of globally unique [identifier](https://en.wikipedia.org/wiki/Identifier "Identifier") that enables an [entity](https://en.wikipedia.org/wiki/Entity "Entity") to be identified in a manner that is [verifiable](https://en.wikipedia.org/wiki/Verifiable_credentials "Verifiable credentials"), persistent (as long as the DID controller desires), and does not require the use of a centralized [registry](https://en.wikipedia.org/wiki/Domain_name_registry "Domain name registry").[[1]](https://en.wikipedia.org/wiki/Decentralized_identifier#cite_note-W3_did-core-1) DIDs enable a new model of decentralized [digital identity](https://en.wikipedia.org/wiki/Digital_identity "Digital identity") that is often referred to as [self-sovereign identity](https://en.wikipedia.org/wiki/Self-sovereign_identity "Self-sovereign identity") or [decentralized identity](https://en.wikipedia.org/wiki/Decentralized_identity "Decentralized identity").[[2]](https://en.wikipedia.org/wiki/Decentralized_identifier#cite_note-DID-EU-2) They are an important component of [decentralized web](https://en.wikipedia.org/wiki/Decentralized_web "Decentralized web") applications.

Source: [WikiPedia](https://en.wikipedia.org/wiki/Decentralized_identifier)

### W3C: Decentralized Identifiers (DIDs) v1.0
#### Core architecture, data model, and representations

[Decentralized identifiers](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers) (DIDs) are a new type of identifier that enables verifiable, decentralized digital identity. A [DID](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers) refers to any subject (e.g., a person, organization, thing, data model, abstract entity, etc.) as determined by the controller of the [DID](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers). In contrast to typical, federated identifiers, [DIDs](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers) have been designed so that they may be decoupled from centralized registries, identity providers, and certificate authorities. Specifically, while other parties might be used to help enable the discovery of information related to a [DID](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers), the design enables the controller of a [DID](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers) to prove control over it without requiring permission from any other party. [DIDs](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers) are [URIs](https://www.w3.org/TR/did-core/#dfn-uri) that associate a [DID subject](https://www.w3.org/TR/did-core/#dfn-did-subjects) with a [DID document](https://www.w3.org/TR/did-core/#dfn-did-documents) allowing trustable interactions associated with that subject.

Each [DID document](https://www.w3.org/TR/did-core/#dfn-did-documents) can express cryptographic material, [verification methods](https://www.w3.org/TR/did-core/#dfn-verification-method), or [services](https://www.w3.org/TR/did-core/#dfn-service), which provide a set of mechanisms enabling a [DID controller](https://www.w3.org/TR/did-core/#dfn-did-controllers) to prove control of the [DID](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers). [Services](https://www.w3.org/TR/did-core/#dfn-service) enable trusted interactions associated with the [DID subject](https://www.w3.org/TR/did-core/#dfn-did-subjects). A [DID](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers) might provide the means to return the [DID subject](https://www.w3.org/TR/did-core/#dfn-did-subjects) itself, if the [DID subject](https://www.w3.org/TR/did-core/#dfn-did-subjects) is an information resource such as a data model.

This document specifies the DID syntax, a common data model, core properties, serialized representations, DID operations, and an explanation of the process of resolving DIDs to the resources that they represent.

Source: [W3C DID CORE Spec Document](https://www.w3.org/TR/did-core/)

## Concerns

I am particularly concerned about the idea of 'private webs', particularly those built solely upon blockchains - leading to, what many may consider to be 'unintended consequences'.  Intended or otherwise, the consideration is that its best to advoid unwanted consequences.

As the [DID methods registry](https://github.com/w3c/did-spec-registries/tree/main/methods) somewhat already demonstrates; there has seemingly been a rush to obtain namespaces; and this may in-turn illustrate what may be considered, problematic circumstances.  For instance; the Namespace defined as [did:health](https://github.com/w3c/did-spec-registries/commit/347608e6903fd2c9cc867e6949a86f615f1db266) refers to the information noted below

```json

{
  "name": "health",
  "status": "registered",
  "verifiableDataRegistry": "DID Health",
  "contactName": "support",
  "contactEmail": "support@did.healthcare",
  "contactWebsite": "https://www.did.healthcare/",
  "specification": "https://github.com/didhealth/health-did-resolver/blob/main/doc/did-method-spec.md"
}

```

Then, when going to https://www.did.healthcare/ the site is redirected to: https://rimmo.co/ (an e-commerce shop)

In the example for the term [DID:ID](https://github.com/w3c/did-spec-registries/commit/1fdde3119fd968b496f5ab104994eea09222ffef), the method is registered to Mastercard.

```json 

{
    "name": "id",
    "status": "registered",
    "verifiableDataRegistry": "ID Service",
    "contactName": "Mastercard",
    "contactEmail": "",
    "contactWebsite": "https://idservice.com/en/contactus.html",
    "specification": "https://github.com/Mastercard/did-methods/blob/master/id.md"
}

```

The Below [record](https://github.com/w3c/did-spec-registries/commit/6d12ed8bee1120f72dc9fdcc44ffc0cf8890e8d5) describes itself. further information is available [here](https://github.com/microsoft/did-ccf/blob/main/DID_CCF.md)
```json
{
    "name": "ccf",
    "status": "registered",
    "verifiableDataRegistry": "CCF",
    "contactName": "Microsoft",
    "contactEmail": "bmurdoch@microsoft.com",
    "contactWebsite": "https://www.microsoft.com/en-us/research/project/confidential-consortium-framework/",
    "specification": "https://github.com/microsoft/did-ccf/blob/main/DID_CCF.md"
  }
```

The [ion](https://github.com/w3c/did-spec-registries/blob/main/methods/ion.json) methods refers to the project by [identity.foundations](https://identity.foundation/ion/)
```json
{

"name": "ion",

"status": "registered",

"verifiableDataRegistry": "Bitcoin",

"contactName": "Various DIF contributors",

"contactEmail": "",

"contactWebsite": "",

"specification": "https://github.com/decentralized-identity/ion-did-method"

}
```

The complete list will be analysed and derivative information will be provided once that has occurred. 

It may well be that the way the `did` specification has been developed, are not fit for purpose for PCT-ONT; yet, it may also be found that my fears, are not supported by the technical characteristics of what has been produced; regardless of how some people might seek to use them.  The thing about making tools - for example - a hammer - is that, its impossible to ensure that they're only used for good purposes - as tools can be used for good or evil.

More investigation is required to better evaluate the decentralised nature of decentralised identifiers, etc. 

As noted, I was personally very emotional about the global rollout of 'vaccine passports' and the entire situation disaffected me greatly, as such i do have personal views - which i am entitled to have and express - whilst seeking to do so, clearly - rather than doing otherwise.

*NOTE:  These works are only loosely coupled to the psychological concept of [Disassociative Identity Disorder](https://en.wikipedia.org/wiki/Dissociative_identity_disorder) particularly with respect to the [[Webizen]] and [[PeaceInfrastructureProject]] scope of works which actively seeks to address [[SocialAttackVectors]] related issues; including but not limited to Human Trafficking ( Note: [UNODC: Anti-Human Trafficking Manual for Criminal Justice Practitioners](https://www.unodc.org/unodc/en/human-trafficking/2009/anti-human-trafficking-manual.html) ) and other forms of abuse that are closely tied to Severe Mental Illness as defined by the [DSM](https://en.wikipedia.org/wiki/Diagnostic_and_Statistical_Manual_of_Mental_Disorders) publications; including but not limited to DID.*

##### jurisdictions 

In-order to support inter-national world order, whereby each UN recgonised member state (at a minimum) is supported in being provided the means to manage their electronic affairs domestically; particularly where such sorts of requirements relate to such things as legislative records, then i am unsure how a URI structure registered by an organisation like Mastercard may reasonably support the [[Centricity]] related requirements - at this time...  Perhaps there's something that i've missed and simply do not understand, however, it is not obvious to me how these solutions provide support for sovereignty in any meaningful way broadly. 

### Possible Solutions - A Draft Note

The underlying methodology for defining how a decentralised ontology (PCT-ONT) standards compatible system works, may simply provide a series of ontological references that in-turn enable the client (end users) to get the resource from whatever network they prefer to use themselves; thereby, leading to a situation where the information can be collected from a range of different networks, rather than solely being available on one network (ie: DID:ID).

The belief is that these systems are going to play a major role in the future; and the question becomes, whether or not it has anything to do with PCT or whether and/or how other systems either support DIDs as a primary solution or via some sort of backwards compatibility related solutions - as may be required by [[Webizen]] for 'wallet' functionality.