# Expanded Corpora Generation
## **Open Source Tool**
 ***by [Betterment Labs](http://www.bettermentlabs.com/)***

### Project Definition
1. Create tools that allow for Expanded Corpora generation easily
2. "" for Phoneme Corpora


### Definitions
*Corpora*:  a collection of written or spoken material in machine-readable form, assembled for the purpose of studying linguistic structures, frequencies, etc.

***Expanded Corpora:*** 
 - Word *(written or verbal** *)*
 - Word occurrence frequency
 - Word broken down into phonemes (component sounds)
 - Use indices [?] (where word was used — à la Strong's Concordance Numbers)
 - Words occurring before & after word:
	 - two words before, two words after (and frequency of occurrences)
	 - count all end-of-sentence punctuation as a word (i.e. period "."; exclamation point "!"; question mark "?" or others, depending on language)

**verbal only will be added later*

***Phoneme Corpora?***
- primary spelling of phoneme
- alternative spellings
- word associations
	- either as its own database or as part of Word corpora above
- associated phonemes (preceding and seceding ... one or two in either direction?)
- phoneme frequencies?

### Concerns/Questions:
- Particular language concerns: 
	- non-phonetic languages
	- unwritten languages
- database structure:
	-  Mark Davies's Corpora use a [SQL RDS-structured](https://corpus.byu.edu/faq.asp#x4)
	- Would a graph database be appropriate?
- how to handle accents
- how to account for conjugations/declensions/etc in corpora

### Relevant Materials & Resources:
- [Mark Davies's Corpora](https://corpus.byu.edu/)
- Graph Databases:
	- [https://gun.eco/#step1](https://gun.eco/#step1)
	 - [https://medium.com/@reinman/create-your-first-wormhole-in-javascript-ef88d8c66fad](https://medium.com/@reinman/create-your-first-wormhole-in-javascript-ef88d8c66fad)
	- [https://neo4j.com/developer/graph-database/](https://neo4j.com/developer/graph-database/)
- [Google paper on generating Corpora](: https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36801.pdf)
- English Phonemes:
	- https://www.youtube.com/watch?v=xiqUVnXExTQ
	- https://www.dyslexia-reading-well.com/support-files/the-44-phonemes-of-english.pdf
	- http://sites.fas.harvard.edu/~interns/eng101quiz/definitions.html
	- Graphemes: http://www.speechlanguage-resources.com/support-files/soundstographemesguide2.pdf
	- 


### Proposed Approach:
- Used New Testament Greek
	- Reasons:
		- [Strong’s Concordance](https://en.wikipedia.org/wiki/Strong%27s_Concordance) has data we can check our results against
		- Source texts are easily accessible online
		- Team members have experience with language
		- Non-Roman alphabet gives a start for non-Roman alphabet languages
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTA4MTAzOTc3MCwzNzk3NjUxMzksLTc0Nz
UzMDYwOSw4OTUwNjM0MzYsMTIwNDEwNjE3MCwxMTQxNTUzOCwx
NzQwNTg5ODg3XX0=
-->