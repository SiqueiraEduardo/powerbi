<h1 align="left">POWER BI</h1>

###

<p align="left">Estudos voltados para o desenvolvimento de Power bi</p>

###

<h2 align="left">RLS</h2>

###

<p align="left">Nessa pasta temos um controle básico de Segurança em Nivel de linha onde a hierarquia está disposta em colunas desta forma:</p>

###

<div align="center">
  <img height="600" src="https://github.com/SiqueiraEduardo/powerbi/blob/main/RLS/Imagens/Imagem_RLS_01.png?raw=true"  />
</div>

###

<p align="left">Onde o Níve_1, por óbvio é o maior e o 8 o menor e o mais granular (Não se Repete)<br><br>Esse arquivo e o Arquivo de Vendas simulado para teste de propagação do RLS foram criados usando a Lib Faker do Python. <br>o código usado está no arquivo<br>https://github.com/SiqueiraEduardo/powerbi/blob/main/RLS/HierarquiaFake.ipynb</p>

###

<h3 align="left">Funcionamento na Prática</h3>

###

<p align="left">Com esse formato de dados em hierarquia é bem simples a implementação. Bastando apenas 2 passos dentro do Power BI<br><br>1 - Concatenar todas as colunas<br>*  Página Inicial -> Transformar Dados -> Editor Avançado e implemente o código de concatenação conforme imagem abaixo.</p>

###

<div align="center">
  <img height="200" src="https://github.com/SiqueiraEduardo/powerbi/blob/main/RLS/Imagens/Imagem_RLS_02.png?raw=true"  />
</div>

###

<p align="left">Obs: Se atente ao nome do passo anterior que deve ser o mesmo nome dentro de AddColumn<br><br>O Resultado esperado pós concatenação é esse:</p>

###

<div align="center">
  <img height="900" src="https://github.com/SiqueiraEduardo/powerbi/blob/main/RLS/Imagens/Imagem_RLS_03.png?raw=true"  />
</div>

###

<p align="left">Feito isso implemente a regra de RLS tal qual a imagem abaixo:</p>

###

<div align="center">
  <img height="200" src="https://github.com/SiqueiraEduardo/powerbi/blob/main/RLS/Imagens/Imagem_RLS_04.png?raw=true"  />
</div>

###

<p align="left">Com isso seu RLS está pronto, se leu até aqui meus muito parabéns</p>

###
