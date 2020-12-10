L�MPADA: Pacote de Recursos do Segundo HAREM
--------------------------------------------

Este pacote est� acess�vel a partir de http://www.linguateca.pt/HAREM/PacoteRecursosSegundoHAREM.zip, e inclui os principais recursos criados no �mbito do Segundo HAREM, uma avalia��o conjunta em reconhecimento de entidades mencionadas em portugu�s.

Conte�do
1.	Organiza��o do Segundo HAREM
2.	Colec��es
3.	Programas de avalia��o
4.	Corridas dos sistemas
5. 	Agradecimentos
 
Estrutura do pacote
Este pacote cont�m tr�s directorias, que compreendem os recursos indicados em 2., 3. e 4., respectivamente.
coleccoes/ 
programas/
corridas/

1. Organiza��o do Segundo HAREM
-------------------------------

1.1 Organizadores
O HAREM � organizado pela Linguateca (http://www.linguateca.pt). 
A equipa do Segundo HAREM foi: Diana Santos, Cl�udia Freitas, Hugo Oliveira, Paula Carvalho e Cristina Mota.

1.2 Datas importantes do Segundo HAREM
Primeira chamada para participa��o: Outubro de 2007
Envio das corridas pelos participantes: Abril de 2008 
Resultados oficiais: Setembro de 2008

1.3 Documenta��o
A documenta��o integral do Segundo HAREM, que inclui as directivas das v�rias pistas, pode ser consultada em:  
Cristina Mota & Diana Santos (eds.). Desafios na avalia��o conjunta do reconhecimento de entidades mencionadas: O Segundo HAREM. Linguateca, 2008. http://www.linguateca.pt/LivroSegundoHAREM/

1.4 Como citar o Pacote de Recursos do Segundo HAREM
Este pacote deve ser referido como "L�MPADA - Pacote de Recursos do Segundo HAREM" (http://www.linguateca.pt/HAREM/PacoteRecursosSegundoHAREM.zip)


2. Colec��es douradas e colec��o HAREM
--------------------------------------

2.1 Colec��o HAREM
Esta colec��o, colSegundoHAREM.xml, � constitu�da por um conjunto de 1040 documentos que os sistemas tiveram de anotar no Segundo HAREM. 

Em colSegundoHAREM-meta.xml, fornecemos os meta-dados relativos � fonte e ao tipo de cada texto, inequivocamente identificado pelo valor do DOC (identificador do documento).
Em seguida, uma breve explica��o sobre os diferentes valores usados:

VARIANTE: PT (Portugal) ou BR (Brasil)

TIPO_TEXTO: classifica��o que procura dar uma indica��o geral sobre o g�nero do texto. No Segundo HAREM, identific�mos
	- Not�cia: factos ou acontecimentos recentes. Associada � maior parte das not�cias de jornal encontra-se, al�m disso, a indica��o da sec��o do jornal de que foram retiradas, no atributo SECJORNAL de FONTE. 
	- Did�ctico: textos educativos, tais como artigos de enciclop�dia, material acad�mico, cartilhas, etc.
	- Opini�o: artigos de opini�o ou ensaios. 
	- Blogue: textos que tamb�m expressam opini�es, mas normalmente num estilo menos formal. Os blogues foram subcategorizados em "blogue pessoal", no caso de o texto ter sido escrito num registo pessoal, "blogue jornal�stico", no caso de o texto ter um registo pr�ximo do de um artigo de jornal, e "blogue humor�stico". 
	- Perguntas: textos n�o articulados em termos de conte�do; trata-se de perguntas (artificiais), especificamente usadas na tarefa de avalia��o de sistemas de resposta autom�tica a perguntas (QA@CLEF). 
	- Perguntas faq (FAQ): perguntas e respostas encontradas em p�ginas de "Frequently Asked Questions".
	- Entrevista: di�logos
	- Legislativo: textos legais
	- Liter�rio: textos retirados de obras liter�rias
	- Promocional: textos publicit�rios ou de promo��o
	- Texto privado manuscrito

FONTE: informa��o sobre a origem/fonte do texto.
	NOME classifica o canal de publica��o: nome do jornal, t�tulo do livro, t�tulo do s�tio, colec��es anteriores, etc. 
	AUTOR designa o nome do autor, quando este � conhecido
	DATA-CRIACAO indica a data de publica��o
	DATA-OBTENCAO indica a data de quando o texto foi acedido
	REFERENCIA inclui o URL
	TITULO designa o nome do excerto particular do texto
	SECJORNAL cont�m a sec��o do jornal � qual as not�cias pertencem: Cien_Tecn_Educ, COTIDIANO, Cultura, Desporto, Diversos, Economia, ESPORTE, FOLHATEEN, FOLHINHA, ILUSTRADA, Local, Mundo, Nacional/Brasil, Nacional/Portugal, OPINI�O, REVISTA_DA_FOLHA, Sociedade, TURISMO, TV_FOLHA


2.2 Colec��es douradas (CD)
�ltima revis�o: 10 de Novembro de 2008.

CD do Segundo HAREM: 129 documentos extra�dos da colec��o HAREM, cujas entidades mencionadas foram manualmente anotadas, de acordo com as directivas do HAREM cl�ssico, em CDSegundoHAREM.xml.

CD do TEMPO (um subconjunto da CD do Segundo HAREM): 30 documentos em que as EM, al�m de conterem a informa��o da CD do Segundo HAREM, tamb�m foram manualmente anotadas de acordo com as directivas do TEMPO, com vista a uma an�lise mais fina das EM temporais e sua normaliza��o, em CDSegundoHAREM_TEMPO.xml.

CD do ReRelEM (um subconjunto da CD do TEMPO): 12 documentos em que as EM, al�m de conterem as informa��es das CD anteriormente referidas, tamb�m t�m associada a informa��o das rela��es sem�nticas que estabelecem com as demais EM no texto, as quais foram manualmente anotadas de acordo com as directivas do ReRelEM, em CDSegundoHAREM_ReRelEM.xml.

As tr�s colec��es podem ainda conter coment�rios, assinalados pelo atributo COMENT, que disponibilizamos para estudos futuros. Segue-se uma breve descri��o dos valores poss�veis que este atributo pode tomar:

a) 2/3: a classifica��o da EM (categoria, tipo ou subtipo) n�o foi feita por consenso, mas por maioria.
b) DUVIDA_DIRECTIVASTEMPO: casos de TEMPO em que as anotadoras tiveram d�vidas, geralmente associadas a diferentes interpreta��es poss�veis das directivas do TEMPO (cujos proponentes estavam impossibilitados de esclarecer, dado que tamb�m eram participantes do Segundo HAREM).
c) INDEP: diz respeito � pista do ReRelEM, e indica que a rela��o reconhecida pelas anotadoras n�o pode ser inferida atrav�s da informa��o fornecida pelo texto.
d) futuro: diz respeito � pista do ReRelEM, e indica que a rela��o reconhecida pelas anotadoras apenas acontecer� no futuro (dado que essa rela��o, de acordo com a informa��o do texto, ainda n�o aconteceu).


3. Programas de avalia��o
-------------------------
Vers�o: 11 de Novembro de 2008.

3.1 Requisitos
- M�quina virtual Java 1.6 ou superior
- gawk (para a avalia��o dos atributos estendidos de TEMPO)
- R vers�o 2.7.1 ou superior (para a gera��o dos relat�rios individuais)

3.2 Instala��o e utiliza��o
- Extrair o conte�do deste pacote para onde for pretendido
- Fazer a invoca��o dos programas a partir da directoria Av_HAREM_XML

3.3 Manual de utiliza��o
- O manual, em HTML, encontra-se na directoria Av_HAREM_XML/docs
- Exemplos de utiliza��o adicionais e notas para compila��o do c�digo encontram-se em programas/Leiame_programas.txt

3.4 Licen�as
Todos os programas desenvolvidos no HAREM s�o distribu�dos com base na licen�a BSD (ver programas/LICENSE.txt).
Al�m disso, distribu�mos os seguintes programas externos, na directoriaprogramas/externos, e que t�m as suas pr�prias licen�as:
- Jdom (http://www.jdom.org), cuja licen�a Apache-style open source est� inclu�da no ficheiro LICENSE.txt do pacote jdom-1.1.zip 
- JGraph (http://www.jdom.org), cuja licen�a LGPL est� inclu�da no ficheiro LICENSE do pacote jgraph-latest-lgpl-src.jar


3.5 Servi�o SAHARA
De notar que o conjunto de programas de avalia��o usados no Segundo HAREM tamb�m pode ser utilizado atrav�s do servi�o SAHARA (Servi�o de Avalia��o HAREM Autom�tico), dispon�vel em http://www.linguateca.pt/HAREM/ (escolher "Avaliador").


4. Corridas dos sistemas participantes
--------------------------------------

10 sistemas participaram no Segundo HAREM e cada sistema p�de enviar, no m�ximo, 4 corridas. As corridas que disponibilizamos neste pacote (na directoria corridas/) s�o, para cada sistema: 

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

O nome dos ficheiros indica o n�mero do participante (atribu�do pela organiza��o), o n�mero da corrida e pode ainda ter o sufixo _corr, que indica que a participa��o sofreu pequenas altera��es (como por exemplo a altera��o da codifica��o de caracteres ou a reatribui��o do atributo DOCID aos documentos).

5. Agradecimentos
-----------------

A Linguateca � financiada pelo governo portugu�s e pela Uni�o Europeia (FEDER e FSE) no �mbito do contrato POSC/339/1.3/C/NAC.
Agradecemos a Caroline Hag�ge, Nuno Mamede e Jorge Baptista pela introdu��o da pista do TEMPO, a Nuno Cardoso pelo desenvolvimento do SAHARA, assim como a David Cruz, Lu�s Miguel Cabral e Lu�s Costa pelo seu apoio em diferentes tarefas ao longo do Segundo HAREM. Queremos tamb�m agradecer a todos os participantes do Segundo HAREM por nos terem autorizado a distribuir as corridas inclu�das no presente pacote.

