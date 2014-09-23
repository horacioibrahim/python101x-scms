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
  
  **Pros**
  
  Captura de erros fáceis de passarem despecebidos como erros de digitação, etc.
  
  **Contras**
  
  pylint não é perfeito. Para tirar vantagem dele, nós iremos precisar algumas vezes de: 
  a) escrever uma solução de contorno b) suprimir essas mensagens C) melhorá-lo
  
  *Decision*
  Certifique-se de rodar o pylint em seu código. Oculte os avisos se eles forem inapropriados
  assim que outros avisos importantes passem despercebidos.
  
  Para suprimir os avisos você pode configurar com um comentário de uma linha
  
  ```
  dict = 'alguma coisa' # Mau ideia... pylint: disable=redefined-builtin
  ```
  
  Os avisos pylint são identificados por um código alfanumérico (c0112) e um nome simbólico
  (empty-docstring). Prefira o nome simbólico nos novos códigos ou quando estiver atualizando 
  um código existente. 
  
  Se o motivo para a supressão não é clara para o nome simbólico adicione um explicação.
  
  Suprimindo desta forma tem a vantagem de que nós poderemos facilmente pesquisar por supressões
  e revistá-las.
  
  Você pode uma lista de avisos do pylint executando ```pylint --list-msgs```. Para ter mais 
  informações sobre uma mensagem em particular use ```pylint --help-mgs=C6409```.
  
  Prefira ```pylint: disable``` a antigo forma já depreciada ```pylint: disable-msg```.
  
  Avisos para argumentos não....

