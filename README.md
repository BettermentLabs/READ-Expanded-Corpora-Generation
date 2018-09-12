# Expanded Corpora Generation
## **Open Source Tool, part of the [READ! Toolkit](http://read-toolkit.com/)**
 ***by [Betterment Labs](http://www.bettermentlabs.com/)***

### Definitions
*Corpora*:  a collection of written or spoken material in machine-readable form, assembled for the purpose of studying linguistic structures, frequencies, etc.

***Expanded Corpora:*** 
 - Word *(written or verbal** *)*
 - Word broken down into phonemes (component sounds)
 - Word occurrence frequency
 - Use indices [?] (where word was used — a la Strong's Concordance Numbers)
 - Words occurring before & after word:
	 - one word before, one word after
	 - five word sequences (two words on either side)
	 - Q: how to handle sentence beginnings/ends
		 - does it matter if a word frequently begins/ends a sentence?

**verbal only will be added later*

***Phoneme Corpora?***
- primary spelling
- alternative spellings
- word associations
- associated phonemes (preceding and seceding)
- frequencies?

Project Needs:
Design, develop and test with potential customers an expert system component to build an expanded

corpora (as described previously) from text, audio and video files for any written language.

Concerns/Questions
— handling non-phonetic written vs. verbal language
— design database
— what libraries we want/need
— how to handle accents
— how to account for conjugations/declensions/etc in corpora

  

Existing Materials:

[https://corpus.byu.edu/](https://corpus.byu.edu/)

  

Steps:

1 — figure out data needs & best structure to handle

2 —


Proposed Plan:

Used New Testament Greek (Strong’s Concordance has these we can check our results against:  
[https://en.wikipedia.org/wiki/Strong%27s_Concordance](https://en.wikipedia.org/wiki/Strong%27s_Concordance))

Source texts are easily accessible online

  

Database questions:

[https://gun.eco/#step1](https://gun.eco/#step1)

[https://medium.com/@reinman/create-your-first-wormhole-in-javascript-ef88d8c66fad](https://medium.com/@reinman/create-your-first-wormhole-in-javascript-ef88d8c66fad)

[https://neo4j.com/developer/graph-database/](https://neo4j.com/developer/graph-database/)


From Mark Davies:
**4. What software is used to index, search, and retrieve data from these corpora?**

We have created our own corpus architecture, using [Microsoft](http://www.microsoft.com/) [SQL Server](http://www.microsoft.com/sqlserver/) as the backbone of the relational database approach. Our proprietary architecture allows for [size](https://corpus.byu.edu/size.asp), [speed](https://corpus.byu.edu/speed.asp), and very good scalability that we don't believe are available with any other architecture. Even complex queries of the more than 560 million word COCA corpus or the 400 million word COHA corpus typically only take two or three seconds. In addition, because of the relational database design, we can keep adding on more annotation "modules" with little or no performance hit. Finally, the relational database design allows for a [range of queries](https://corpus.byu.edu/queries.asp) that we believe is unmatched by any other architecture for large corpora.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc0MDU4OTg4N119
-->