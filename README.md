# DataWarehouse_DataViz-VestibularUFSC

## Data Visualization
- [Link Dashboard PowerBI](https://app.powerbi.com/view?r=eyJrIjoiMWE5MzI0MmQtYWVjNC00N2JhLTlmMDEtMWZjZjllNDU0Yzc3IiwidCI6ImZhNzk1MzFjLThjZTUtNGJkMy05N2VlLTI0NWU2ZWUyNjZiOCJ9&pageName=ReportSection)

## SOFTWARES
- UniController
- HeidiSQL
- Pentaho Data Integration
- SQL Power Architect
- Power BI


## PROJETO
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


## ARQUIVOS:
- Back-end (informações necessárias para acessar o banco de dados, pasta com os
scripts/arquivos do kettle utilizados no ETL, modelagem dimensional);
- Front-end (informações necessárias para acessar a área de apresentação dos
dados);

## Instruções

- Criar uma conexão MySQL local , no meu caso foi usado o UniController para criar a conexão.

- Usando um gerenciador de bases de dados MySQL (HeidiSQL)  e conectar na conexão MySQL.

- Abrir o dump dos dados do vestibular no gerenciador de bases de dados.

- Usar o Script_Criacao_DW para criar criar a tabela de Fato e Dimensões do DataWarehouse, mas ainda sem nenhum dado.

- Com a modelagem criada no HeidiSQL foi usado o Spoon (Pentaho Data Integration) para a execução das etapas de ETL, conectar na mesma conexão SQL do DataWarehouse e da fonte de dados do vestibular.

- No Spoon é usado a conexão em sql para puxar os dados do vestibular, executar as transformações e depois fazer a carga nas respectivas dimensões e fato do banco de dados do DataWarehouse.

- O arquivo dw_ufsc_com_dados.sql contém o DataWarehouse populado com os dados após a Etapa de Carga


## MODELAGEM:
- Modelagem Relacional do banco de dados da fonte
![Modelo Relacional](https://github.com/nicolasantero/DW-VestibularUFSC_DataWarehouse_DataViz/blob/main/Modelos/modelagem_relacional.png?raw=true)
- Modelagem Dimensional do DataWarehouse
![Modelo Dimensional](https://raw.githubusercontent.com/nicolasantero/DW-VestibularUFSC_DataWarehouse_DataViz/main/Modelos/modelagem_DW.JPG?raw=true)

