# Site de Suporte T.I.

Este repositório contém todos os arquivos que compõem o Site de Suporte TI, que tem como objetivo notificar a T.I. sobre problemas recorrentes em sala de aula de maneira rápida e dinâmica.

Isso é feito por um processo automatizado que leva informações de data e hora, identificador de sala e problema comum a uma planilha, por meio de uma API chamada ao clique de botões.

### Requisitos do projeto

Para que fosse possível o processo foram utilizados:
 - html: estrutura do site
 - css: estilização do site
 - javascript: captação e envio dos dados para planilha
 - sheetdb: api que liga planilha ao site

### login.js

Este arquivo é responsável por criar logins únicos para poder acessar o site e enviar o *dado identificador* da sala ao index.js. Caso uma sala nova deva ser acrescentada deve ir para a lista de salas `const salas = []`

### index.js

O index captura a informação da sala do *Local Storage* e envia por meio da api as informações citadas no começo para a planilha. 
Para evitar chamados repetidos em um curto período de tempo, após um botão ser cliaado um popup fica na tela por *tempo determinado* 

Copyright © 2023 Gedai. Todos os direitos reservados.

