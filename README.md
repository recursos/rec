water meter project - ler o mostrador de um contador de água.

2026-01-11 code frame, box:
```
'''
<h3>Aqui continua um di&aacute;rio do Condominio Carcavelos começado em 2012</h3>
TtEXTOS CAPTURADOS COM A FERRAMENTA pYTHON:
rfind_strings_08.py
module_08.py
IF_DEFS.py
Editando o "filename" para um dos DIÁRIOS extrai a DATA acima de [CONDOMÍNIO ] e o testo a seguir este até uma "régua" ----... ou ====...
Abrir com Notepad++, converter para UTF-8 e juntar ao existente
ex:
D:\Hobby2024\CONDO_make>py>text2024.txt rfind_strings_08.py

---------------------------------------------------------------------------------
2026-01-08
┌───────┐
│SUCESSO│
└───────┘
"D:\Hobby2026\CONDO_make\rfind_strings_08.py" mais
"D:\Hobby2026\CONDO_make\modules_08.py"
Funcionam bem com ambos os tipos de "DATA STRING"
uso:
D:\Hobby2026\CONDO_make>py>text2026.txt rfind_strings_08.py
'''
import re
from IF_DEFS import *
from pprint import pprint
from modules_08 import *
# -----------------------------------------------
# -----------------------------------------------
WORD = '[CONDOMÍNIO]'
CONDO_PATTERN = '\[CONDOMÍNIO\]'
DIARIO_FILE = r"D:\PESSOAL\DOCs\DIARIOS\2025diario.html" # copy with Notepad++
print(f'{DIARIO_FILE=}')

if USE_FILE_AS_SOURCE:
    with open(DIARIO_FILE, "r", encoding='utf8') as f:
        src = f.read()
    # print(contents)
count = src.count(WORD)
print((f'(occurrences {WORD}:'), src.count(WORD))

# locate CONDO token, save to a list
condo_ix_list = f_all(CONDO_PATTERN, src)
if PRINT_CONDO_IX: print(f'{condo_ix_list=}')
# procurar 2024MAI20 etc.
# pattern = r"(\d{4}\W{3}\d{2}).*"#.*$)"#, re.MULTILINE) "
# pattern = r"(\d{4}[a-zA-Z]{3}\d{2}).*"# OK
pattern = r"(\d{4}[a-zA-Z]{3}\d{2}).*|(\d{4}-\d{2}-\d{2}).*"
dates_ix_list = list(f_all(pattern, src))
if PRINT_TYPE: print(f'{type(dates_ix_list)}')
if PRINT_DATES: print(f'{dates_ix_list=}')

```
2021-10-31 usei:
github:
  is_project_page: false
na tentativa de fazer desaparecer o "View in Github"


Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/rec2022/rec/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
