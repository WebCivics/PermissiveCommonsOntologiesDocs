
Below is a document that was produced in connection to the brief works on the schema-generator group. 

#### SchemaGen CG Info

[W3C Schema Gen CG](https://www.w3.org/community/schema-gen/) 

Original List: [W3C Schema-Gen](https://lists.w3.org/Archives/Public/public-schema-gen/)
Chat Group: [https://gitter.im/w3cg-schema-gen](https://gitter.im/w3cg-schema-gen) 

### Discovery Related updated notes

An ontology has been found that provides some level of functionality that relates to the concept below.  In another related posts on the [W3C Schema-Gen](https://lists.w3.org/Archives/Public/public-schema-gen/) a poorly communicated illustration relating to discovery (therefore also decentralising search) was briefly noted... 

#### The Document about a Discovery Solution

Original Link: [Google Doc](https://docs.google.com/document/d/13VXBVte-ixR2Ryc9v1g4g2ayk4pkYDHU4hKp_AMpwzA/edit)

**IDEA RE:  PROJECT GROUP - SCHEMA GEN**

INTRODUCTION

The Web of Data provides structured data-level interactivity via WWW using RDF related tools and standards.  The means to resource & identify these tools is challenging for newcomers. 

The use of RDF Tooling is more diverse than is traditional for developers.  Individuals working within libraries, digital agencies and other areas of society should be able to use RDF tools to assist with the development of the Web Of Data.  Developers on the other hand should be able to find, resource and contribute towards the development of RDF tools for use in their own projects and that of others.

This project seeks to produce a decentralised discovery tool for making discoverable, and finding RDF tools on the web.

PROBLEM

The development of RDF has occurred over several years.  Whilst information about tooling is available online in many cases tooling links are either dead, point to unmaintained software and are difficult to find. Categories of online resources include; but are not limited to,

-   Sparql EndPoints
    
-   Ontologies
    
-   Visualisation Services
    
-   Schema Generator 
    
-   Server Platforms
    
-   IDEs
    
-   Graph Databases
    
-   Organisations
    
-   Projects  

IDEA - Upgrade robots.txt / sitemap.xml - functionality - Using RDF

Historically, tools have been discovered and added by an agent to a list of available software. Overtime these lists have often become old with dead links, links to now defunct software or links to software that has continued to be developed under another name/brand/webLocation.  

In the interests of continued support for community development a means is to be defined in which the creation, collation and collection of semantic web tools can be made available using an RDF based solutions.

CONSIDERATION

If a standard filetype were more easily discoverable by clients (ie: indexing sites, software seeking RDF resource, etc. etc.) then the means to better script interactivity with Sparql endpoints is amongst the possible benefits.  Other benefits include improved identification of available software/services/documents.  This in-turn results in a consideration that perhaps the underlying notion is one of updating the underlying robots.txt file to enhance search in a distributed manner for offers and web-services.  This would provide a remarkable upgrade to Web 3.0 related functionality overall.

CONCEPTUAL METHOD (1)

The first mandate is to ensure community members are encouraged to provide links and references to existing services manually.  The way of doing this has been defined at the present stage to be by way of a [Spreadsheet](https://docs.google.com/spreadsheets/d/19IEgvdvwl_EOGhmIFinVQu4OerRojeje8PaZWGvoO4Q/edit#gid=0) that is being developed to identify the initial scope of this undertaking and to produce the ontology needed for others to submit tools to the search solution. 

STEP 1: Define ontological structure and requirements.

The development of schema will provide the means for projects to author project descriptions which can be represented using RDF via 3rd party sites and agents. To do this; the creation of a list of online tools is suggested as an approach to identify the ontological requirements for a search and update mechanism. Where schemaorg does not have appropriate references for service discovery, suggestions can be made for updating schemaorg ontology to support these frameworks.

As noted above: A [Spreadsheet](https://docs.google.com/spreadsheets/d/19IEgvdvwl_EOGhmIFinVQu4OerRojeje8PaZWGvoO4Q/edit#gid=0) is being developed to identify the initial scope of this undertaking and to produce the ontology needed for others to submit tools to the search solution. 

STEP 2: Map Requirements to Ontology.

An ontological tool should be developed to assist people to visually produce valid schemaorg mark-up via a web based tool.

STEP 3: Figure out tooling for production of Information about available offer. 

Once the file has been created, the next step is figuring out how the owner/operator of the hosting environment can upload the information to their hosting environment and make that file easily discoverable. 

Environments include;

-   GitHub (and similar)
    
-   Linux based servers
    
-   Other Servers
    
-   Consumer devices (inc. mobile phones)
    

STEP 4: Figure out how to provide indexing.

If the average size of a robots.rdf file is 10Kb (noting github robots.txt file ~30Kb @1376 lines) and the total number of websites is 1.15 billion, then the total size of the file would be ~1.4 Terabytes.

Once language is taken into account, this number drops dramatically. However this is one of many facets that may be considered to reduce the total size of the file dramatically.

Facets may include; Language, Type, Reputation, Location. 

It is also important to note that any one services platform would likely only suit one genre of website. As such, the total indexable file-suite for any particular type of web-services provider is in-turn likely to decrease substantially again both due to the % marketPlace using the method; and, the means to discriminate based on the type of website being provided.

STEP 4: Figure out how to provide indexing. (concept 1 ipfs / “quins”? )

The theory about ‘quins’ was raised as a potential method to identify from a system point of view, which graph the quad / triple should be added to for propagation of the data into the discovery process. 

This method has later been considered in-practical as it would diminish the means for a solution to grow.

A decentralised method such as IPFS could provide the means to distribute standardised services tools for providing means to add the indexing file (service discovery) to something that is easily accessible. 

The ledger protocol looks for appropriate files and indexes based upon the @context information.  The means of doing this is via a descriptor on the file that points to the purpose of the resource; for example,
```

{

“@context” : “SparqlEndPoint” 

“Ipns” : “[hash]”

“ServiceDecription” : “[https://w3id.org/sparqlendpoints](https://w3id.org/sparqlendpoints)”,

“Reputation” : “[https://user123.reputationmanager.org/mysparqlendpoint](https://user123.reputationmanager.org/mysparqlendpoint)”,

“Distribution” ; “[private]/[public]”

  

"@context": "[http://schema.org/](http://schema.org/)”,

  "@type": "Encyclopedia",

  "name": "DbPedia",

  “url”: “[https://dbpedia.org/sparql](https://dbpedia.org/sparql)”

  "domain": "dbpedia.org",

"signature": {

    "type": "LinkedDataSignature2015",

    "created": "2017-02-18T08:54:19Z",

    "creator": "https://depedia.com/webmaster/keys/3",

    "domain": depedia.org",

    "nonce": "b5fb6904",

    "signatureValue": "WsCvvhWFSezgAwnUi9OqJoDuXhtq+38OuU68A/NNAFIX6lEYSFSERgStOtu9MRe+6fpzFnYO7Vvp9wLLM+JlEqMa6zgiXGwjpqQ158Q0frxYVyQx0akWeomLwnvWckT4OiHuWWA7iZ96mXXlQRMDQnE3hW9PqRZpc6ZdDKsXc7g="

}

```


In this example, local software would identify that the distributed file = SparqlEndPoint, adding the @context information to the ledger describing the offering available at that URL.

The Reputation predicate is both decentralised and able to provide information about whether or not to trust the offer provided in the @context RDF statement.  The reputation service may identify whether the service is active, whether complaints have been made about the service or whether it's a bad actor. 

The signature value (provided as an RSA example) may certify the provider account with the reputation provider and end-client with verification of their transmission to the intended end-point.

ONTOLOGY SELECTION

The search tool will aim to produce recommendations required for Schemaorg to provide the ontology required for the tool.  However by design any ontology tool could be used to support the method.

sameAs frameworks can be used to identify other services that provide similar services based on separate ontologies.  A problem is that the ‘lookup service’ providing interface to the ledger (discovery) is not necessarily the same as the RDF service providing a description of the service.  Herein, two separate functions are considered; and whether or how these are supported is part of the question.


USE CASES
-  User has mobile phone. They’d like to make services discoverable from their Phone or Provider.

-  User has shared-hosting service.  The hosting provider provides access to shared service.

-  User has shared-hosting service.  The hosting provider provides no-access to shared service.

-  User has VPS service.  They’ve got an operating system, how’s that work.

-  User is advertising via GitHub - how’s that work

-  User is advertising via Social Network - The social network has an API.

-  Vendor wants to get paid via Advertising. They’d prefer it if that could be included.

-  Vendor wants to get paid via Subscription. They’d prefer it if that could be included.

-  Vendor requires an account. But they’d like to advertise that offer to people.

-  Vendor requires an account. They need the credentials.

-  Service can do a request - but it’ll need to be checked by others - can you give us a request to process?  (and then either rejected or provided revocable permission)

-   Hosting Service is becoming Decommissioned; lets notify user and offer migration

-   Decentralised App Stores

Other Groups

-   Credentials CG (inc. Verifiable Claims)
-   RWW CG
-   WOT CG
-   SchemaOrg CG
-   WebPayments
-   RDF
-   Privacy