# DW-VestibularUFSC_DataWarehouse_DataViz

PROJETO
1. Analisar o modelo do sócio acadêmico do vestibular da Coperve de
2008 a 2012 com vistas à implementação de um Data Mart para
suporte a seguinte análise;

	- Apoiar a secretaria do estado de SC na avaliação do desempenho nas disciplinas dos
	  candidatos das escolas públicas do estado, comparando com as escolas privadas e
	  federais.

2. Criar um esquema estrela (modelo dimensional) para suportar as
análises;

3. Definir o projeto físico para o Data Mart, seguindo padronização,
estabelecer uma área de transição para o processo de ETL;

4. Criar o Front End do Data Mart em uma ferramenta OLAP

ARQUIVOS:
– Back-end (informações necessárias para acessar o banco de dados, pasta com os
scripts/arquivos do kettle utilizados no ETL, modelagem dimensional, requisitos,
documentação sobre criação dos indicadores/medidas e tudo que possa ser
necessário para para o back-end);
– Front-end (informações necessárias para acessar a área de apresentação dos
dados, link acesso a ferramenta, usuário, senha, documento de especificação e tudo
que possa ser necessário para o front-end);
- Fonte de dados (Banco de dados em MySQL (dump) do Vestibular da UFSC de 2008 a 2012, Divisoes de administrativas de Santa Catarina de novembro 2012);



Criar uma conexão MySQL local , no meu caso foi usado o UniController para criar a conexão.

Usando um gerenciador de bases de dados MySQL (HeidiSQL)  e conectar na conexão MySQL.

Abrir o dump dos dados do vestibular no gerenciador de bases de dados.

Usar o Script_Criacao_DW para criar criar a tabela de Fato e Dimensões do DataWarehouse, mas ainda sem nenhum dado.

Com a modelagem criada no HeidiSQL foi usado o Spoon (Pentaho Data Integration) para a execução das etapas de ETL, conectar na mesma conexão SQL do DataWarehouse e da fonte de dados do vestibular.

No Spoon é usado a conexão em sql para puxar os dados do vestibular, executar as transformações e depois fazer a carga nas respectivas dimensões e fato do banco de dados do DataWarehouse.

O arquivo dw_ufsc_com_dados.sql contém o DataWarehouse populado com os dados após a Etapa de Carga


