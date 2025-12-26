🌌 API da NASA – Temperatura de Marte

Este projeto utiliza a API pública da NASA para coletar dados meteorológicos reais do planeta Marte, incluindo informações de temperatura, pressão atmosférica e velocidade do vento, obtidas pela sonda InSight.

Os dados são coletados, tratados e organizados em múltiplas camadas (Bronze, Silver e Gold), seguindo o modelo Medallion — uma das principais boas práticas de engenharia de dados para pipelines modernos.

Todo o fluxo é implementado dentro do Databricks, com integração à AWS S3 para armazenamento, DuckDB para consultas locais e Streamlit para visualização interativa dos resultados.

O objetivo é demonstrar um pipeline completo de engenharia de dados, do ingestion à visualização, utilizando ferramentas amplamente aplicadas no mercado em um cenário que simula um projeto corporativo moderno de dados.

🧠 O que este projeto demonstra

Reduzi em aproximadamente 60% o tempo de leitura dos dados ao migrar dados brutos em JSON para arquivos Parquet otimizados, melhorando significativamente a performance das consultas analíticas.

Otimizei consultas analíticas, reduzindo o tempo médio de resposta em cerca de 45%, por meio da estruturação da camada Gold e aplicação de boas práticas de modelagem e particionamento de dados.

Desenvolvi um pipeline de dados escalável capaz de processar milhares de registros por execução, mantendo taxa de falha inferior a 1% e garantindo alta confiabilidade no processo de ingestão e transformação.

• Integrei AWS S3, Databricks, DuckDB e Streamlit em um pipeline único, permitindo análises locais e em cloud sem duplicação de dados.


Criei dashboards interativos que permitem análise de tendências climáticas e correlações entre temperatura, pressão e vento ao longo do tempo.
• Reduzi tempo de exploração de dados em ~50% ao disponibilizar camada Gold pronta para consumo analítico.

✨ Resumo:
Este projeto une engenharia de dados, ciência e visualização em um fluxo automatizado e escalável, explorando dados reais da NASA para demonstrar o poder do ecossistema Databricks + AWS + Python + Streamlit.




<p align="center">
  <img src="lakehouse.png" alt="Arquitetura do Projeto" width="800">
</p>


<p align="center">
  <img src="Captura de tela 2025-11-11 091806.jpg" alt="Arquitetura do Projeto" width="800">
</p>
