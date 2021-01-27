# Instruções

- Criar uma conexão MySQL local , no meu caso foi usado o UniController para criar a conexão.

- Usando um gerenciador de bases de dados MySQL (HeidiSQL)  e conectar na conexão MySQL.

- Abrir o dump dos dados do vestibular no gerenciador de bases de dados.

- Usar o Script_Criacao_DW para criar criar a tabela de Fato e Dimensões do DataWarehouse, mas ainda sem nenhum dado.

- Com a modelagem criada no HeidiSQL foi usado o Spoon (Pentaho Data Integration) para a execução das etapas de ETL, conectar na mesma conexão SQL do DataWarehouse e da fonte de dados do vestibular.

- No Spoon é usado a conexão em sql para puxar os dados do vestibular, executar as transformações e depois fazer a carga nas respectivas dimensões e fato do banco de dados do DataWarehouse.

- O arquivo dw_ufsc_com_dados.sql contém o DataWarehouse populado com os dados após a Etapa de Carga