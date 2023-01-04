(HMKD)
The concept of knowledge docs, is a document format that incorporates knowledge graph references with the english structured (technically unstructured) text. 

The Purpose of this is to support the means through which #AI can process the intended meaning of a document, and in-turn also produce a linked-graph in relation to the intended statements of that document.  

### Requirements

1. An ability to define a file-structure strategy.  
	The file-strategy needs to be made able to work with an existing file format (ie: markdown) and provide complimentary file that provides support for the hypermedia knowledge document functionality. 
2. Archivability and longevity
	The file-format should be able to be independently processed by future technology long after the authors of the artifacts are deceased.  (ie: in 100 years time).  
3. Formats
	The knowledge document structure should support different use-case related formats.  
	
	For example; a 'master' version format, 
	- may include raw quality copies of information as to store the original information in the highest possible format.  
	- may include private and/or sensitive information (ie: journalism related source materials) that is not intended to be distributed with the 'public' version of the derivative work.
	- may include production related information, where the conversations, editorial history, information about how a work was produced and which entities were involved in making contributions and decisions along the way, etc.
	
	A Distribution version format; May be defined,
	- To work on a particular device or system
	- As a Translation via some sort of means to be consumed in other languages or medium (ie: braille)
	- to have Reduced the quality (ie: resolution) or format of any media attachments
	- to make use of alternative vocabulary models
	
4. Functionality Considerations
	- The ability to support RDF Links for the intended meaning of words and concepts.
	- The ability to support a capacity to review historical changes that have been made to a document; perhaps via GIT based SVN methods.
	- An ability to support attribution for content that is sourced from 3rd parties. 
	- An ability to support a description of a license provided in relation to a document; and independently also, in relation to any other artifacts that are provided in the document.
	  
5. An ability to define an extensible way for managing vocabularies.
	- Use of Semantic Web related principals, whilst seeking to mitigate historical challenges.
	- Objective is to provide support for 'permissive commons'
	
6. A way to assert statements in relation to the costs incurred (time, resources, etc) to produce and or work on an artifact; and in-turn also, link those statements with those of others related to any contributed artifacts associated with a 'body of work'.  

Quick notes on how this might be applied using the current [[Documentation Method]]

#### Obsidian
a. It would be useful to create an obsidian plugin that could look-up terms and provide a means to link a RDF URI or a http-uri with a secondary RDF Uri (RDF Statements) to the concept being described.  
b. #LinkeDataTags that could use RDF to describe the tag concept (rdf statements)
c. As the existing documentation method consumes markdown (.md) files, and it is difficult to provide support for the extended functionality via the .md file itself; perhaps the way it could be done is to provide some sort of ```.meta ``` file (not necessarily that extension) that has the same file-name and internally references the file; via a link provided in the ```.md``` file, as to provide a means for a parser to be provided the functionality to represent the information via a render. 

NOTE: The  Gatsby library uses react, which supports #GraphQL but not natively #RDF.  Whilst i am unsure if the version control method using Git could be supported for presentation; the information could be provided as a link to the commit information.   

### Gatsby 
The Gatsby Presentation library would need to be updated to process the metadata files. 


