🌌 Projeto: Pipeline de Dados — NASA API com Databricks Lakehouse

Este projeto tem como objetivo construir um pipeline de engenharia de dados completo, desde a ingestão até a visualização, utilizando a arquitetura Lakehouse no Databricks.
Os dados são coletados da API pública da NASA, armazenados em camadas no Amazon S3 e processados no Databricks, com suporte adicional de DuckDB para consultas locais e Streamlit para visualização.

⚙️ Arquitetura e Fluxo de Dados
O fluxo segue o modelo Medalhão (Bronze → Silver → Gold):

Ingestão
Linguagem: Python
Ferramentas: Databricks Notebooks
Fonte de dados: NASA API
Armazenamento inicial: Amazon S3 (Bronze)
Arquivos salvos em formato JSON e convertidos para Parquet

Armazenamento e Load
Amazon S3 para camadas Bronze/Silver/Gold
DuckDB para testes e consultas locais
Controle de permissões via AWS IAM

Transformação
Databricks SQL e PySpark
Limpeza, tratamento e normalização dos dados (Silver)
Criação de métricas e agregações (Gold)

Visualização
Streamlit conectado à camada Gold





Dashboards interativos mostrando os principais insights dos dados da NASA

