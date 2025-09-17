<!DOCTYPE HTML>
<html>
<head>

<meta http equiv="Content Type" content="text/html; charset=utf-8">
<title>2025 GEO X (html)</title>

<style type="text/css">
.toDo {  COLOR: blue}
.report {  COLOR: magenta}
.personal { FONT STYLE: italic}
.personal { color: blue; BACKGROUND: lightGray}
.grayed {COLOR: gray}
.highlite {BACKGROUND: yellow}
.toDo2 {BACKGROUND COLOR: black}
.toDo2 {color: white}
.negative {BACKGROUND COLOR: black; color: white}
a:link { color: lightblue}
a:visited { color: red}
a:hover {
    TEXT DECORATION: underline; FONT WEIGHT: bold
}
th, td {
  padding: 10px;
}
</style>
</head>
<body>
<hr>
<!-- para mudar de "positive" para "negative" e vice-versa 
problema que sugiu com o uso de high-contrast em Windows 10
-->
<style type="text/css">
/* Browser specific (not valid) styles to make preformatted text wrap */		

pre {
 white-space: pre-wrap;       /* css-3 */
 white-space: -moz-pre-wrap;  /* Mozilla, since 1999 */
 white-space: -pre-wrap;      /* Opera 4-6 */
 white-space: -o-pre-wrap;    /* Opera 7 */
 word-wrap: break-word;       /* Internet Explorer 5.5+ */
}
a:link { color: lightblue}
a:visited { color: red}
</style>
<!-- para mudar de "positive" para "negative" e vice-versa 
problema que sugiu com o uso de high-contrast em Windows 10
-->
<div style = "text-align:center; position:fixed; left:0px">
       <button onclick = "to_positive()">  
            <h3>White</h3>
        </button> 
		<button style = "background-color: black; color: white"; onclick = "to_negative()">  
            <h3>Black</h3>
        </button> 
    
</div>          
        <script> 
		 function to_negative() {
			document.body.style.background = "black";
			document.body.style.color = "white";
		 }
		 function to_positive() {
			document.body.style.background = "white";
			document.body.style.color = "black";
		 }
        </script>
</script>

<table style="width: 640px; border: 1px solid #ff0000">
<tbody>
<tr>
<td>

<hr>
<pre>
=================================================================================
INDEX:
2925SET08 [DICA EXTRAORDINÁRIA: dev tools ANDROID ]
=================================================================================
</pre>
<h3>2025 GEO X slides etc.<br>
</h3>
<pre>===================================================================================
2025-09-04 Quinta-feira
Encomenda: Power Point com figuras e legendas de:
"D:\eBOOKS\Hist+Bio + War\Maps and Their Place in Mesopotamia etc.epub"

Ancient Perspectives: Maps and Their Place in Mesopotamia, Egypt, Greece and Rome
 Richard J. A. Talbert
 University of Chicago Press, Maps and Their Place in Mesopotamia, Egypt, Greece, and Rome; The Kenneth Nebenzahl Jr. Lectures in the History of Cartography, 2014

para acordar a classe!

Folder de trabalho:
"D:\Hobby2024\2025_GEO_X"
-----------------------------------------------------------------------------------
Para fixar a tenção:
https://www.chasingraiders.com/media-resources
"Archaeologist Dr. David West Reynolds" consultor nos filmes de Indiana Jones,
meter foto tipo Indiana Jones!
-----------------------------------------------------------------------------------
Pegar em:
file:///D:/Hobby2024/2025_GEO_X/text/ch10.html
e editar comprimindo - reduzindo, fica a faltar a tradução.

Esta tentativa não vai longe, pq acabo por me perder nas sources.
Agora vou tentar fazer o HTML manualmente, com um esqueleto "repetido" e copiado do original, e depois LINKS para as imagens.
00_geo.html

agora para mão ficar com linhas longas e imagens curtas, meter tudo numa TABLE?
Grande dificuldade em fazer "responsive", copiei de @2020diario.html

"Image caption width to same as image" (SO)
melhor:
"Image captions and wrapping" (SO)
Perguntar ao CHAT-4o
HTML, CSS:
 Image caption width to same as image and aligned with image.
 The image is centered on a larger page.
 
 html

Copy Code
<div class="image-container">
    <img src="your-image-url.jpg" alt="Description of image" class="centered-image">
    <p class="image-caption">This is the caption for the image.</p>
</div>

css

.image-container {
    text-align: center; /* Center the content */
}

.centered-image {
    max-width: 100%; /* Responsive image */
    height: auto; /* Maintain aspect ratio */
}

.image-caption {
    width: fit-content; /* Width of the caption matches the image */
    margin: 0 auto; /* Center the caption */
    display: block; /* Make the caption a block element */
}
mas depois de estar qusae a funcionar, até centrava as imagens, mas o texto expandia-se para lá da imagem, depois de mexer passou a não cntrar nada!
e não percebo porquê!

Agora fui ao ARIA - e voltei a meter pés pelsa mãos!
Posso ficar horas nisto.
Que tal fazer qq coisa que percebo, como TABLES simples? baseadas nso DIARIOS?
-----------------------------------------------------------------------------------
EW como organizar para copiar as "strings" sem refazer os tags?
O melhor é ter um esqueleto, depois ir por "replace" de tokens.

A lista dos links das tentativas:
https://logs.rf.gd/geo/images
https://logs.rf.gd/geo/01_geo.html
https://logs.rf.gd/geo/index-en.html
https://logs.rf.gd/geo/index.pt.works.00.html
https://logs.rf.gd/geo/index_1.html
https://logs.rf.gd/geo/index_2.html
https://logs.rf.gd/geo/index_last.html
https://logs.rf.gd/geo/w3.css

o ARIA deu-me isto:

<!DOCTYPE html> <html lang="en">
<head> <meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Geo Resources Links</title>
<style> body { font-family: sans-serif; line-height: 1.6; margin: 20px; background-color: #f4f4f4; } h1 { color: #333; border-bottom: 2px solid #333; padding-bottom: 10px; } ul { list-style-type: none; padding: 0; } li { background-color: #fff; margin-bottom: 10px; padding: 15px; border-radius: 5px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); } a { color: #007bff; text-decoration: none; font-weight: bold; } a:hover { text-decoration: underline; color: #0056b3; } </style> </head>
<body>

<h1>Geo Resources</h1>
<ul>
    <li><a href="https://logs.rf.gd/geo/images">images</a></li>
    <li><a href="https://logs.rf.gd/geo/01_geo.html">01_geo.html</a></li>
    <li><a href="https://logs.rf.gd/geo/index-en.html">index-en.html</a></li>
    <li><a href="https://logs.rf.gd/geo/index.pt.works.00.html">index.pt.works.00.html</a></li>
    <li><a href="https://logs.rf.gd/geo/index_1.html">index_1.html</a></li>
    <li><a href="https://logs.rf.gd/geo/index_2.html">index_2.html</a></li>
    <li><a href="https://logs.rf.gd/geo/index_last.html">index_last.html</a></li>
    <li><a href="https://logs.rf.gd/geo/w3.css">w3.css</a></li>
</ul>
</body> </html>

Abrir com:
https://logs.rf.gd/beogeo_links.html
-----------------------------------------------------------------------------------
experimentar:
https://responsively.app/
para testar etc.
baixei:
ResponsivelyApp-Setup-1.17.0.exe não presta

===================================================================================
2925SET08 [DICA EXTRAORDINÁRIA: dev tools ANDROID ]
┌───────────────────────────┐
│ DICA EXTRAORDINÁRIA:      │
│ nO cHROME ACEDER Inspect  │
│ ao ANDROID                │
└───────────────────────────┘
Mentioning this because you mentioned "when developing".

You can control the mobile device via your Chrome Desktop Browser.

Visit:
chrome://inspect/#devices

PORVEZES É DIFÍCIL DE "PEGAR", INSISTIR|

on your desktop. And Inspect the device that's connected to your desktop. Agree when asked for permission.

You should now see a full fledged Devtool window for the current page on mobile device.

Now, Use the hard reload shortcut (Cmd+Shift+R) on desktop to do hard reload on mobile device!
===================================================================================
2025SET08
Qual é a imagem com maior width? 739px

Uma AI fixe:
HTML, CSS: is it possible to get the width of a image?
https://www.eye2.ai/c/34fd065a-4bbe-4fb5-a8b1-a449791fd1ef

respondem simultaneamente várias AIs, dá para comparar, o LINK da resposta pode ser salvo, é free - que é que paga estas coisas?
-----------------------------------------------------------------------------------
Vou encomendar um Python ao AI:
PYTHON:
A script that:
- reads "strings.txt" file with this format:
 (int_1, [string_11, string_12]),
 (int_2, [string_21, string_22]),
 etc.
 (int_n, [string_n1, string_n2]),
º carefull with strip(',', strings may  contain ',' and '\n' and UTF-8 chars!
- reads "template.txt" file with this format:
"template text... string_1_placeholder template text string_2_placeholder... template text"
- generates a file with "n" lines, each line is the template with the placeholders replaced by the strings from strings.txt
- saves the generated file.

https://www.eye2.ai/c/80aa06a8-0e21-4c92-9ec4-7ee42558bed4

Um grande problemas é que os "tokens" contêm "," de modo que o Strip(',') falha que se farta!! nova questão:

https://www.eye2.ai/c/4cc68f15-20f9-43e0-912d-710d87090f25

O formato do ficheiro tokens.txt que usei é tão complicado que lixa tudo! o split(',') só causa desastres!
E no entanto se usar uma list-of-lists deve ser fácil!
Vou pedir ao ARIA:
PYTHON, json
Give me a example of a json file for a "list of lists" with 3 items with 2 string items each, like:
[["string1", "string2"],["string12", "string22"],["string13", "string23"]]

Grande luta com a formatação do JSON - como são strings, não posso ter "line breaks com ENTER"
Mas parece-me que se usar como "template" num módulo, até me safo!!
Em alternativa, processar uma a uma
Falta-me escrever o ficheiro HTML com os place-holders!
-----------------------------------------------------------------------------------
2025SET10
Depois
de marrardurante horas,vou fazer um "caso muito simples" a ver se entendo.

PYTHON
- um tuple com strings placeholders:
- uma string "nody" com "place holder" dentro dela;
- uma list of lists com strings que vão substituir os placeholders;
um loop para dentro de cada lista de strings trocar os placeholders 

ex: placeholders("_IMG_SRC", "_IMG_ALT_", "_DESCRITIVO_")
body = "<a href='_IMG_SRC_' alt='_IMG_ALT_'>_DESCRITIVO_</a><br>"
elements = [
['images/potato.png', 'a potato', 'what is a potato?'],
 ['images/tomato.png', 'a tomato', 'what is a tomato?']
 ]

depois da substituição deve ficar:
output = "<a href='images/potato.png' alt='a potato'>what is a potato?</a><br>
<a href='images/tomato.png' alt='a tomato'>what is a tomato?</a><br>
"

O DuckAI deu logo a resposta curta e certa, FUNCIONOU!
┌───────┐
│SUCESSO│
└───────┘
"D:\Hobby2024\2025_GEO_X\trials\PYTHON\Qwen\repl_tokens.py"
o que falta:
- tratar da primeira "caption" no topo do ficheiro! que não tem image - ou em alternativa, inventar uma image, género um globo?

O primeiro que tentei, era muito escuro:
["images/globe.jpg", "dlovan-666-ZQ2KT2J4uDI-unsplash", "Práticas de mapeamento do antigo Egito, Mesopotâmia, Grécia e Roma"],

-----------------------------------------------------------------------------------
[COMO REFRESCAR A PÁGINA]
Parece que funciona anexar uma query ao URL, depois faz sempre hard reload da página?
Não, só da primeira vez! teria de mexer no "geo_links.html" todos os dias!
Ou usar JS para modificr o URL, parece mais decente!

https://logs.rf.gd/geo/table_DIV_BLOCK.html?userId=5
ir mexendo na página a ver se funciona!
-----------------------------------------------------------------------------------
2025SET12
Bolas, há "" por todo o lado ex:
"Práticas de mapeamento do antigo Egito, Mesopotâmia, Grécia e Roma"<br>
como evitar isto? Vou explicar ao Chat-4n:

PYTHON:
This script:

for placeholder, value in zip(placeholders, element):
	item_output = item_output.replace(placeholder, value)

where element = ["one", "another"] replaces the placeholder qith the strings, but it includes the double quotes.
How to make it replace the strings without the quotes?
Pois, é que tinha:
[SOLVED]
"_DESCRITIVO_" em vez de _DESCRITIVO_!

Quanto a aparecerem "single quotes2, começa logo mal;
body:
'<div class="block">
                <img src="_IMG_SRC_"  class="img-centered" alt="_IMG_ALT_" />
        <p>
        _DESCRITIVO_
    </div>
<hr>
'
pq é que o "body" tem plicas??
Mas abrindo em Notepad.exe mostra plicas, apago-as e salvando, as plicas desaparecem, visualamnete o Notepad++
não parece ter nenhuma diferença! yau! MISTÉRIOS!
E isto só acontece mesmo em "table_DIV_BLOCK_body.txt", n-ao nos "header" e "footer"
-----------------------------------------------------------------------------------
2025SWT12
Agora, com TABELA simples.
Uma pequena complicação: os nomes do ficheiros alteram-se:
era: "table_DIV_BLOCK_header.txt" => "TABLE_header.txt"
Como lidar com isto? ler de um ficheiro de configuração?
https://www.geeksforgeeks.org/python/how-to-write-a-configuration-file-in-python

[General]
header = TABLE_header.txt
body = TABLE_body.txt
footer =TABLE_footer.txt
-----------------------------------------------------------------------------------
2025SWT13
Forcing a Fresh Reload (Workaround)

window.location.href = window.location.href.split('?')[0] + '?cache=' + new Date().getTime();
Onde colocar e como chamar?
┌───────┐
│SUCESSO│ o DuckDuckAI deu-me a resposta OK, ver:
└───────┘ "D:\Hobby2024\2025_GEO_X\geo_links.html"

-----------------------------------------------------------------------------------
Para fazer:
- meter "strings.json" num folder comum
- idem o Python
-ter 3 (ou mais) folders para os vários estilos, com os "config.cfg".
- meter o output.html no folder root, onde terei também  batch files de lançamento do mesmo Python referindo-se a cada folder de estilo.
NÃO É ASSIM, MAS QUASE! terei de ter <args> na linha de comando?

As CLI que apanhei, são más demais - talvez não haja uma boa solução fora de tkinter?
Tenho de me contentar com talvez manter o Fython no root, e multiplas cópias de "strings.json", chamar de cada folder > pu ..\repl_tokens.py
Mas é mau que se farta!
Ou embeber no repl_tokens.py "..\strings.json" e output = 
HEI, meter "..\strings.json" no config.sfg!!! FUNCIONOU!
-----------------------------------------------------------------------------------
A interpretação do mapa de Babilónia:
https://neareast.jhu.edu/directory/paul-a-delnero

===================================================================================
2025SET15
Vamos a ver se consigo produzir POWER POINT com Python...
https://python-pptx.readthedocs.io/en/latest/community/faq.html
┌───────┐
│SUCESSO│ "D:\Hobby2024\2025_GEO_X\geo\PPTX\aria_00.py"
└───────┘ usa ..\images e data.json (== strings.json mas sem HTML tags)
Invocar o LiberOffice depois de gerar o PPTX:

"C:\Program Files\LibreOffice\program\soffice.exe" presentation.pptx

batch file sugerido:
ECHO
py aria_00.py
"C:\Program Files\LibreOffice\program\soffice.exe" presentation.pptx

recursos,Git2013

mail: noreply@forumdalinha.pt
pass: Git2013fdl
user: rec2022
https://rec2022.github.io/rec/ tem lá um README sobre OPTO ou RTP

ruibackup,Git(2)2021
===================================================================================

</pre>
</td>
</tr>
</tbody>
</table>
</html>
