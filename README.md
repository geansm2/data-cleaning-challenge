#  Data Cleaning Challenge

Este repositório é uma demonstração prática de habilidades de **Data Wrangling** e **Limpeza de Dados**. 

Enquanto a maioria dos cursos foca em modelos de IA, este projeto foca na etapa que consome 80% do tempo de um Cientista de Dados: **limpar o caos**.

##  O Desafio
O arquivo `vendas_brutas_caos.csv` simula uma extração real de um sistema legado, contendo:
- **Datas em múltiplos formatos** (ISO, BR, e erros como mês 13).
- **Inconsistência de strings** (Espaços extras, casing misturado, delimitadores errados).
- **Valores monetários sujos** (Símbolo de R$, separadores de milhar e decimal trocados).
- **Duplicidade de registros** e valores nulos (`NaN` e `NULL`).

##  Abordagem Técnica
No notebook `Cleaning_Process_Report.ipynb`, implementei uma pipeline de higienização que:
- Utiliza **Expressões Regulares (Regex)** para normalizar nomes de clientes.
- Aplica lógica de **Conversão de Moeda** resiliente para transformar strings em floats.
- Trata inconsistências temporais através de técnicas de interpolação e tratamento de erros.
- Documenta cada **Trade-off** de negócio tomado durante a limpeza.

##  Estrutura do Repositório
- `Cleaning_Process_Report.ipynb`: Relatório detalhado com o "Antes e Depois" dos dados.
- `vendas_brutas_caos.csv`: O dataset bruto utilizado no desafio.

---
**Este projeto demonstra que a qualidade dos insights depende diretamente da qualidade da limpeza dos dados. "Garbage in, garbage out".**
