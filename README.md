LÂMPADA: Second HAREM Resource Package
--------------------------------------

This package can be downloaded from http://www.linguateca.pt/HAREM/PacoteRecursosSegundoHAREM.zip, and includes the main resources created in the scope of Second HAREM, a joint evaluation on named entity recognition in Portuguese.

Contents
1.	Second HAREM organization
2.	Collections
3.	Evaluation programs
4.	System runs
5. 	Ackowledgments
 
Package structure
This package has three directories, corresponding to 2., 3. and 4. respectively.
coleccoes/ 
programas/
corridas/

1. Second HAREM organization
----------------------------

1.1 Organizers
HAREM is organized by Linguateca (http://www.linguateca.pt). 
People involved in the Second HAREM: Diana Santos, Cláudia Freitas, Hugo Oliveira, Paula Carvalho and Cristina Mota.

1.2 Second HAREM main dates
First call of participation: October, 2007
Submission period: April, 2008 
Official results: September, 2008

1.3 Documentation
The complete documentation of the Second HAREM, including the guidelines to all tracks, is available from: 
Cristina Mota & Diana Santos (eds.). Desafios na avaliação conjunta do reconhecimento de entidades mencionadas: O Segundo HAREM. Linguateca, 2008. http://www.linguateca.pt/LivroSegundoHAREM/

1.4 How to cite the present package
This package is available from http://www.linguateca.pt/HAREM/PacoteRecursosSegundoHAREM.zip 
and should be cited as "LÂMPADA - Second HAREM Resource Package" 


2. Golden collections and HAREM collection
----------------------------------------------

2.1 HAREM collection
This collection, colSegundoHAREM.xml, contains a set of 1,040 documents in Portuguese (from Brazil and from Portugal) that the systems had to annotate in the Second HAREM. 

In colSegundoHAREM-meta.xml, we provide meta-data related to the source and kind of each text, uniquely identified by its DOC (document identification) value. Follows the explanation of the values used:

VARIANTE (language variety): PT (Portugal) or BR (Brazil)

TIPO_TEXTO (text type): the classification in text types is a rough indication of the text genre. In Second HAREM we used
	- Notícia (news): facts and recent events. Most news have also associated the newspaper section they appeared in, in the attribute SECJORNAL under FONTE (source)
	- Didáctico (didactic): instructional texts, such as encyclopedia articles, course book snippets, state health instructions, etc.
	- Opinião (opinion): newspaper articles and (academic) essays. 
	- Blogue (blog): these texts also express opinions, but usually in a less formal style. Blogs are also subcategorized in "blogue pessoal" (personal blog), when the text is written in a personal register, "blogue jornalístico" (journalistic blog), when the text is close to a newspaper article, and "blogue humorístico" ("humoristic blogs"). 
	- Perguntas (questions): non-articulated texts; only (artificial) questions, specifically used for evaluation of question answering systems (QA@CLEF). 
	- Perguntas faq (FAQ): questions and answers found in Frequently Asked Questions webpages.
	- Entrevista (interview): consisting of dialogues
	- Legislativo (legal): legal text
	- Literário (literary): from literary works
	- Promocional (promotional): advertisements
	- Texto privado manuscrito (private manuscript)

FONTE (source): information about text origin/source.
	NOME encloses the publication channel: newspaper name, book title, site title, previous collections, etc.
	AUTOR the author when known
	DATA-CRIACAO indicates the publication date
	DATA-OBTENCAO indicates when the text was accessed
	REFERENCIA includes the URL
	TITULO encloses the name of the particular piece of text
	SECJORNAL contains the newspaper section to which the particular news belong: Cien_Tecn_Educ, COTIDIANO, Cultura, Desporto, Diversos, Economia, ESPORTE, FOLHATEEN, FOLHINHA, ILUSTRADA, Local, Mundo, Nacional/Brasil, Nacional/Portugal, OPINIÃO, REVISTA_DA_FOLHA, Sociedade, TURISMO, TV_FOLHA


2.2 Golden collections (GC)
Last revision: November 10th, 2008.

Second HAREM GC: 129 documents from the HAREM collection whose named entities were manually annotated according to HAREM guidelines, in CDSegundoHAREM.xml

TEMPO GC (a subset of Second HAREM GC): 30 documents which in addition to the Second HAREM GC information have also been manually annotated according to the TEMPO guidelines for finer analysis and temporal normalization, in CDSegundoHAREM_TEMPO.xml

ReRelEM GC (a subset of TEMPO GC): 12 documents which in addition to the two types of annotation just referred have also been manually annotated with semantic relations between named entities according to the ReRelEM guidelines, in CDSegundoHAREM_ReRelEM.xml.


These three collections may in addition contain comments signalled by the COMENT attribute, provided for further study. Follows a short description of the possible values of the COMENT attribute:

a) 2/3 -> the NE classification (category, type or subtype) was not assigned by consensus. Rather it was the result of a majority vote.
b) DUVIDA_DIRECTIVASTEMPO -> cases of TEMPO on which the annotators had doubts, generally because of different interpretations of the TEMPO guidelines (whose proposers, as Second HAREM participants, could not be invoked to clarify).
c) INDEP: concerning the ReRelEM track, it indicates that the relation marked by the annotators could not be inferred by the information given by the text.
d) futuro: also concerning the ReRelEM track, it indicates that the relation marked by the annotators will only become actualized in the future.


3. Evaluation programs
--------------------------
Version: November 11th, 2008.

3.1 Pre-requisites
- Any operating system that supports Java 1.6 or a more recent version.
- gawk (to evaluate extended TEMPO attributes).
- R 2.7.1 or a more recent version (to generate individual evaluation reports).

3.2 Installation
- Extract the content of this archive
- Invoke the programs through the directory named Av_HAREM_XML

3.3 Manual
- The manual in HTML (in portuguese) can be found in the Av_HAREM_XML/docs directory
- Additional utilization examples and minimal compilation instructions can be found in programas/Readme_programas.txt

3.4 Licenses
All programs developed within HAREM are distributed under the BSD license (see programas/LICENSE.txt).
In addition, we distribute as well the following external programs, under the directory programas/externos, which have their own licenses
- Jdom (http://www.jdom.org), Apache-style open source license included in file LICENSE.txt in jdom-1.1.zip
- JGraph (http://www.jdom.org), LGPL licence included in file LICENSE in jgraph-latest-lgpl-src.jar


3.5 SAHARA web service 
Note that the whole evaluation setup of Second HAREM is also available through the 
SAHARA Web service. Go to http://www.linguateca.pt/HAREM/, and, in the English interface, choose "Scorer" on the lefthand menu. ["Avaliador" in the Portuguese interface.]


4. Runs submitted to the Second HAREM
--------------------------------------

10 systems participated in the Second HAREM and each system could at most submit 4 runs. 
The runs made available in this package (under corridas/) are, for each system:

Cage2:
partic01_1_corr.xml
partic01_2_corr.xml
partic01_3_corr.xml
partic01_4_corr.xml

DobrEM:
partic03_1_corr.xml

PorTexTO:
partic06_1_corr.xml
partic06_2_corr.xml
partic06_3_corr.xml
partic06_4_corr.xml

Priberam:
partic07_1.xml

R3M:
partic09_1.xml
partic09_2.xml

REMBRANDT:
partic10_1.xml
partic10_2.xml
partic10_3_corr.xml

REMMA:
partic11_1_corr.xml
partic11_2_corr.xml
partic11_3_corr.xml

SEI-Geo:
partic13_1.xml
partic13_2.xml
partic13_3.xml
partic13_4.xml

SeRELeP:
partic15_1.xml

XIP-L2F/XEROX:
partic16_2.xml
partic16_3.xml


The filename identifies the number of the system (assigned by the organization), the number of the run, and the suffix "_corr" indicates that the run suffered minor changes (for example, change of character encoding or renaming of document ID).


5. Acknowledgments
------------------

Linguateca is jointly funded by the Portuguese Government and the European Union (FEDER and FSE) under contract ref. POSC/339/1.3/C/NAC. 
We are grateful to Jorge Baptista, Caroline Hagège and Nuno Mamede for introducing the TEMPO track, to Nuno Cardoso for deploying SAHARA, and to Luís Miguel Cabral, Luís Costa and David Cruz for their support in several other tasks.
We also thank all Second HAREM participants for granting us permission to further distribute their runs. 

