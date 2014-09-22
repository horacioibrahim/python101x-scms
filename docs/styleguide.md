Guia de Estilo Python
========================
Essas regras podem ser encontradas atualizadas em  http://google-styleguide.googlecode.com/svn/trunk/pyguide.html.
Este guia foi traduzido para facilitar a leitura no idioma atual e foi proposto como um guia para os treinamentos 
do curso Python 101x. 

Experiência
------------
O Python é a principal linguagem de script usada no Google. Este guia de estilo é uma lista do que
fazer e o que não fazer para programas em Python.

  [Suprimido parte referente ao settings do Vim]
  
Regras da Linguage Python
--------------------------

#####Lint
  Rode pylint sobre seu código
  
  **Definição**
  pylint é uma ferramenta para localizar problemas no código (bugs) e problemas no estilo em
  código-fontes Python. Ela encontra problemas que são tipacamente capturados por um compilador
  para linguagens menos dinâmicas como C e C++. Por cause da natureza dinâmica do Python alguns
  aviso podem ser incorretos; embora, os avisos falsos possam ser razoalmente frequentes.
  
  *Pros*
  Captura de erros fáceis de passarem despecebidos como erros de digitação, etc.
  
  *Contras*
  pylint não é perfeito. Para tirar vantagem dele, nós iremos precisar algumas vezes de: 
  a) escrever em torno dele b) suprimir essas mensagens C) melhorar isto
  
  *Decision*
  Tenha certeza que você rodou pylint em seu código....

