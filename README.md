🌌 API da NASA – Temperatura de Marte

Este projeto utiliza a API pública da NASA para coletar dados meteorológicos reais do planeta Marte, incluindo informações de temperatura, pressão atmosférica e velocidade do vento, obtidas pela sonda InSight.

Os dados são coletados, tratados e organizados em múltiplas camadas (Bronze, Silver e Gold), seguindo o modelo Medallion — uma das principais boas práticas de engenharia de dados para pipelines modernos.

Todo o fluxo é implementado dentro do Databricks, com integração à AWS S3 para armazenamento, DuckDB para consultas locais e Streamlit para visualização interativa dos resultados.

O objetivo é demonstrar um pipeline completo de engenharia de dados, do ingestion à visualização, utilizando ferramentas amplamente aplicadas no mercado em um cenário que simula um projeto corporativo moderno de dados.

🧠 O que este projeto demonstra

Aplicação prática de conceitos de ETL/ELT dentro da arquitetura Lakehouse.

Integração entre Python, Databricks, AWS e Streamlit em um fluxo de dados real.

Boas práticas de versionamento, governança e visualização de dados.

Capacidade de integração entre ferramentas cloud e open source.

⚙️ Arquitetura e Fluxo de Dados

O pipeline segue o modelo Medallion (Bronze → Silver → Gold), estruturado em quatro etapas principais:

1️⃣ Ingestão

Linguagem: Python

Ferramentas: Databricks Notebooks

Fonte de dados: NASA InSight Weather API

Armazenamento inicial: Amazon S3 (camada Bronze)

Formato: JSON → Parquet

2️⃣ Armazenamento e Load

Camadas: Bronze, Silver e Gold armazenadas no Amazon S3

Banco local: DuckDB para testes e consultas rápidas

Governança: Controle de permissões via AWS IAM

3️⃣ Transformação

Tecnologias: Databricks SQL e PySpark

Processos: Limpeza, padronização e enriquecimento dos dados (Silver)

Resultados: Métricas, agregações e insights prontos para consumo (Gold)

4️⃣ Visualização

Ferramenta: Streamlit

Conexão: Camada Gold

Resultados: Dashboards interativos com os principais indicadores e insights meteorológicos de Marte

✨ Resumo:
Este projeto une engenharia de dados, ciência e visualização em um fluxo automatizado e escalável, explorando dados reais da NASA para demonstrar o poder do ecossistema Databricks + AWS + Python + Streamlit.




<p align="center">
  <img src="lakehouse.png" alt="Arquitetura do Projeto" width="800">
</p>


<p align="center">
  <img src="Captura de tela 2025-11-11 091806.jpg" alt="Arquitetura do Projeto" width="800">
</p>
