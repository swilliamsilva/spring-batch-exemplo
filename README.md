# Spring Boot with Spring Batch Example 1
# Spring Boot with Spring Batch - Aplicação.

## Load CSV to DB
- `http://localhost:8085/load` - Trigger point for Spring Batch
- `http://localhost:8085/h2-console` - H2 Console for querying the in-memory tables.

## H2 Config
- `testdb` - Database.
- `sa` - User
- `password` - Password.

## Motivação
- `Processamento em Batch` 
Processamento de Dados Sincrono utilizado para grandes volumes de dados,
no estilo ENTRADA-PROCESSAMENTO-SAIDA sem intervenção humana.

Voce passa um lote de serviço (job) para processamento o sistema procede a leitura faz a consistência, efetua os cálculos dentro das regras do negócio e gera uma arquivo de saída. 
Aqui no exemplo ele pega ua lista USER.CSV, processa alterações e grava no banco de dados. ´testdb´. 
O exemplo tem poucos dados mas pode ser multiplicado por milhares.

