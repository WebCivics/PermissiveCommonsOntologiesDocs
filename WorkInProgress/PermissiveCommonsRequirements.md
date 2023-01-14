# Permissive Commons Technology (PCT) Requirements.

### Summary

Work is being performed to produce a requirements analysis to inform a design approach as required for an implementation.  The process involves defining [[Requirements]], declaring [[ProblemStatement]] and therefore seeking to define [[PermissiveCommonsTech]].

This is a non-trivial process.  There will be different options that will become exposed; some will deliver 'optional features' (MAY / OPTIONAL) others will define 'requirements' (MUST).

The initial implementation target is the webizen ecosystem. Whilst the work is being done in a manner that seeks to ensure this is not necessarily the sole and exclusive implementation method that is allowed; the complexities that may result in other ecosystems having difficulty implementing these systems, is not of primary concern; although, considered where the requirements to do better are reasonable and do not act to harm underlying principals relating to the Web Civics / Webizen Approach. 

### Introduction

PCT is intended to provide a solution whereby commons resources (including ontologies) become part of the broader 'semantic web' ecosystem that would ordinarily be provided via HTTP via ICANN registered domains; are able to be provided via alternative [[Non-HTTP(s)Protocols]].

The solution seeks to address the following functionality criteria.  

Whilst not all solutions will support the same feature-set, different types of 'permissive commons' will have different requirements.

1. Permissions 
	a. Read
	b. Write
	c. Append
	d. Delete 

2. Version Control
	a. append only
	b. the ability to target a particular version
	c. the ability to delete previous versions
	d. the ability to redirect from previous version links

3. Users and User Groups
	a. The ability to support Agent-centric management
	b. The ability to support user-centric management
	c. The ability to support legal entities (groups)
	d. the ability to vary permissions within groups

4. Semantic Querying
	a. The ability to structure the resource index via ontologies.
	b. the ability to query the protocol based upon ontological terms
	
 5. Network Management
	 a. the ability to prioritise which versions should be stored
	 b. the ability to manage availability (ie: redundancy, retention, replication, etc)
	 c. the ability to provide structured information about the resources used 
	 d. the ability to work with currencies to support economic semantics

6.  