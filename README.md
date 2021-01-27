# DW-VestibularUFSC_DataWarehouse_DataViz

Data Visualization
- [Dashboard PowerBI](https://app.powerbi.com/view?r=eyJrIjoiMWE5MzI0MmQtYWVjNC00N2JhLTlmMDEtMWZjZjllNDU0Yzc3IiwidCI6ImZhNzk1MzFjLThjZTUtNGJkMy05N2VlLTI0NWU2ZWUyNjZiOCJ9&pageName=ReportSection)

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
- Back-end (informações necessárias para acessar o banco de dados, pasta com os
scripts/arquivos do kettle utilizados no ETL, modelagem dimensional, requisitos,
documentação sobre criação dos indicadores/medidas e tudo que possa ser
necessário para para o back-end);
- Front-end (informações necessárias para acessar a área de apresentação dos
dados, link acesso a ferramenta, usuário, senha, documento de especificação e tudo
que possa ser necessário para o front-end);
- Fonte de dados (Banco de dados em MySQL (dump) do Vestibular da UFSC de 2008 a 2012, Divisoes de administrativas de Santa Catarina de novembro 2012);


MODELAGEM:
- Modelagem Relacional do banco de dados da fonte
![Modelo Relacional](https://github.com/nicolasantero/DW-VestibularUFSC_DataWarehouse_DataViz/blob/main/Modelos/modelagem_relacional.png?raw=true)
- Modelagem Dimensional do DataWarehouse
![Modelo Dimensional](https://raw.githubusercontent.com/nicolasantero/DW-VestibularUFSC_DataWarehouse_DataViz/main/Modelos/modelagem_DW.JPG?raw=true)

