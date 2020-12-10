LÂMPADA: Pacote de Recursos do Segundo HAREM
--------------------------------------------

Este pacote está acessível a partir de http://www.linguateca.pt/HAREM/PacoteRecursosSegundoHAREM.zip, e inclui os principais recursos criados no âmbito do Segundo HAREM, uma avaliação conjunta em reconhecimento de entidades mencionadas em português.

Conteúdo
1.	Organização do Segundo HAREM
2.	Colecções
3.	Programas de avaliação
4.	Corridas dos sistemas
5. 	Agradecimentos
 
Estrutura do pacote
Este pacote contém três directorias, que compreendem os recursos indicados em 2., 3. e 4., respectivamente.
coleccoes/ 
programas/
corridas/

1. Organização do Segundo HAREM
-------------------------------

1.1 Organizadores
O HAREM é organizado pela Linguateca (http://www.linguateca.pt). 
A equipa do Segundo HAREM foi: Diana Santos, Cláudia Freitas, Hugo Oliveira, Paula Carvalho e Cristina Mota.

1.2 Datas importantes do Segundo HAREM
Primeira chamada para participação: Outubro de 2007
Envio das corridas pelos participantes: Abril de 2008 
Resultados oficiais: Setembro de 2008

1.3 Documentação
A documentação integral do Segundo HAREM, que inclui as directivas das várias pistas, pode ser consultada em:  
Cristina Mota & Diana Santos (eds.). Desafios na avaliação conjunta do reconhecimento de entidades mencionadas: O Segundo HAREM. Linguateca, 2008. http://www.linguateca.pt/LivroSegundoHAREM/

1.4 Como citar o Pacote de Recursos do Segundo HAREM
Este pacote deve ser referido como "LÂMPADA - Pacote de Recursos do Segundo HAREM" (http://www.linguateca.pt/HAREM/PacoteRecursosSegundoHAREM.zip)


2. Colecções douradas e colecção HAREM
--------------------------------------

2.1 Colecção HAREM
Esta colecção, colSegundoHAREM.xml, é constituída por um conjunto de 1040 documentos que os sistemas tiveram de anotar no Segundo HAREM. 

Em colSegundoHAREM-meta.xml, fornecemos os meta-dados relativos à fonte e ao tipo de cada texto, inequivocamente identificado pelo valor do DOC (identificador do documento).
Em seguida, uma breve explicação sobre os diferentes valores usados:

VARIANTE: PT (Portugal) ou BR (Brasil)

TIPO_TEXTO: classificação que procura dar uma indicação geral sobre o género do texto. No Segundo HAREM, identificámos
	- Notícia: factos ou acontecimentos recentes. Associada à maior parte das notícias de jornal encontra-se, além disso, a indicação da secção do jornal de que foram retiradas, no atributo SECJORNAL de FONTE. 
	- Didáctico: textos educativos, tais como artigos de enciclopédia, material académico, cartilhas, etc.
	- Opinião: artigos de opinião ou ensaios. 
	- Blogue: textos que também expressam opiniões, mas normalmente num estilo menos formal. Os blogues foram subcategorizados em "blogue pessoal", no caso de o texto ter sido escrito num registo pessoal, "blogue jornalístico", no caso de o texto ter um registo próximo do de um artigo de jornal, e "blogue humorístico". 
	- Perguntas: textos não articulados em termos de conteúdo; trata-se de perguntas (artificiais), especificamente usadas na tarefa de avaliação de sistemas de resposta automática a perguntas (QA@CLEF). 
	- Perguntas faq (FAQ): perguntas e respostas encontradas em páginas de "Frequently Asked Questions".
	- Entrevista: diálogos
	- Legislativo: textos legais
	- Literário: textos retirados de obras literárias
	- Promocional: textos publicitários ou de promoção
	- Texto privado manuscrito

FONTE: informação sobre a origem/fonte do texto.
	NOME classifica o canal de publicação: nome do jornal, título do livro, título do sítio, colecções anteriores, etc. 
	AUTOR designa o nome do autor, quando este é conhecido
	DATA-CRIACAO indica a data de publicação
	DATA-OBTENCAO indica a data de quando o texto foi acedido
	REFERENCIA inclui o URL
	TITULO designa o nome do excerto particular do texto
	SECJORNAL contém a secção do jornal à qual as notícias pertencem: Cien_Tecn_Educ, COTIDIANO, Cultura, Desporto, Diversos, Economia, ESPORTE, FOLHATEEN, FOLHINHA, ILUSTRADA, Local, Mundo, Nacional/Brasil, Nacional/Portugal, OPINIÃO, REVISTA_DA_FOLHA, Sociedade, TURISMO, TV_FOLHA


2.2 Colecções douradas (CD)
Última revisão: 10 de Novembro de 2008.

CD do Segundo HAREM: 129 documentos extraídos da colecção HAREM, cujas entidades mencionadas foram manualmente anotadas, de acordo com as directivas do HAREM clássico, em CDSegundoHAREM.xml.

CD do TEMPO (um subconjunto da CD do Segundo HAREM): 30 documentos em que as EM, além de conterem a informação da CD do Segundo HAREM, também foram manualmente anotadas de acordo com as directivas do TEMPO, com vista a uma análise mais fina das EM temporais e sua normalização, em CDSegundoHAREM_TEMPO.xml.

CD do ReRelEM (um subconjunto da CD do TEMPO): 12 documentos em que as EM, além de conterem as informações das CD anteriormente referidas, também têm associada a informação das relações semânticas que estabelecem com as demais EM no texto, as quais foram manualmente anotadas de acordo com as directivas do ReRelEM, em CDSegundoHAREM_ReRelEM.xml.

As três colecções podem ainda conter comentários, assinalados pelo atributo COMENT, que disponibilizamos para estudos futuros. Segue-se uma breve descrição dos valores possíveis que este atributo pode tomar:

a) 2/3: a classificação da EM (categoria, tipo ou subtipo) não foi feita por consenso, mas por maioria.
b) DUVIDA_DIRECTIVASTEMPO: casos de TEMPO em que as anotadoras tiveram dúvidas, geralmente associadas a diferentes interpretações possíveis das directivas do TEMPO (cujos proponentes estavam impossibilitados de esclarecer, dado que também eram participantes do Segundo HAREM).
c) INDEP: diz respeito à pista do ReRelEM, e indica que a relação reconhecida pelas anotadoras não pode ser inferida através da informação fornecida pelo texto.
d) futuro: diz respeito à pista do ReRelEM, e indica que a relação reconhecida pelas anotadoras apenas acontecerá no futuro (dado que essa relação, de acordo com a informação do texto, ainda não aconteceu).


3. Programas de avaliação
-------------------------
Versão: 11 de Novembro de 2008.

3.1 Requisitos
- Máquina virtual Java 1.6 ou superior
- gawk (para a avaliação dos atributos estendidos de TEMPO)
- R versão 2.7.1 ou superior (para a geração dos relatórios individuais)

3.2 Instalação e utilização
- Extrair o conteúdo deste pacote para onde for pretendido
- Fazer a invocação dos programas a partir da directoria Av_HAREM_XML

3.3 Manual de utilização
- O manual, em HTML, encontra-se na directoria Av_HAREM_XML/docs
- Exemplos de utilização adicionais e notas para compilação do código encontram-se em programas/Leiame_programas.txt

3.4 Licenças
Todos os programas desenvolvidos no HAREM são distribuídos com base na licença BSD (ver programas/LICENSE.txt).
Além disso, distribuímos os seguintes programas externos, na directoriaprogramas/externos, e que têm as suas próprias licenças:
- Jdom (http://www.jdom.org), cuja licença Apache-style open source está incluída no ficheiro LICENSE.txt do pacote jdom-1.1.zip 
- JGraph (http://www.jdom.org), cuja licença LGPL está incluída no ficheiro LICENSE do pacote jgraph-latest-lgpl-src.jar


3.5 Serviço SAHARA
De notar que o conjunto de programas de avaliação usados no Segundo HAREM também pode ser utilizado através do serviço SAHARA (Serviço de Avaliação HAREM Automático), disponível em http://www.linguateca.pt/HAREM/ (escolher "Avaliador").


4. Corridas dos sistemas participantes
--------------------------------------

10 sistemas participaram no Segundo HAREM e cada sistema pôde enviar, no máximo, 4 corridas. As corridas que disponibilizamos neste pacote (na directoria corridas/) são, para cada sistema: 

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

O nome dos ficheiros indica o número do participante (atribuído pela organização), o número da corrida e pode ainda ter o sufixo _corr, que indica que a participação sofreu pequenas alterações (como por exemplo a alteração da codificação de caracteres ou a reatribuição do atributo DOCID aos documentos).

5. Agradecimentos
-----------------

A Linguateca é financiada pelo governo português e pela União Europeia (FEDER e FSE) no âmbito do contrato POSC/339/1.3/C/NAC.
Agradecemos a Caroline Hagège, Nuno Mamede e Jorge Baptista pela introdução da pista do TEMPO, a Nuno Cardoso pelo desenvolvimento do SAHARA, assim como a David Cruz, Luís Miguel Cabral e Luís Costa pelo seu apoio em diferentes tarefas ao longo do Segundo HAREM. Queremos também agradecer a todos os participantes do Segundo HAREM por nos terem autorizado a distribuir as corridas incluídas no presente pacote.

