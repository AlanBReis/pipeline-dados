# Projeto de ETL - Combinação de Dados de Duas Empresas

Este projeto tem como objetivo realizar um processo de ETL (Extração, Transformação e Carga) de dados provenientes de duas empresas, "EmpresaA" e "EmpresaB". Os dados da **EmpresaA** estão em formato JSON, enquanto os dados da **EmpresaB** estão em formato CSV. O processo combina essas informações em um único arquivo CSV para facilitar a análise pela equipe de dados.

## Descrição

Este projeto executa os seguintes passos:

1. **Extração (Extract)**:
   - Leitura dos dados da **EmpresaA** a partir de um arquivo JSON.
   - Leitura dos dados da **EmpresaB** a partir de um arquivo CSV.

2. **Transformação (Transform)**:
   - Renomeação das colunas dos dados da **EmpresaB** para torná-las consistentes com os dados da **EmpresaA**.
   - Combinação dos dados das duas empresas em um único conjunto de dados (usando um "join" baseado em chaves comuns).

3. **Carga (Load)**:
   - Salvamento dos dados combinados em um arquivo CSV, pronto para análise.

## Estrutura do Projeto

data_raw/:
    - dados_empresaA.json: Dados da EmpresaA em formato JSON.
    - dados_empresaB.csv: Dados da EmpresaB em formato CSV.

data_processed/:
    - dados_combinados.csv: Dados combinados e transformados.

processamento_dados_desafio.py: Arquivo com a classe `Dados` responsável por processar os dados.


