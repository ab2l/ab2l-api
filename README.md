# Padrão de Interoperabilidade de Dados Jurídicos

## Objetivo

Desenvolver um layout padrão para facilitar a integração entre LegalTechs com o objetivo de reduzir o tempo de integração entre as aplicações e facilitar a troca de informações do ecossistema.

Para isso foi criado um grupo de trabalho com a participção de um conjunto de empresas, que analisou padrões existentes no mercado, como o MNI, padrões de formato de dados, tecnologias adotadas pelas empresas e dados que são trocados.

## Grupo de trabalho
* Daniel Marques @AB2L
* Hugo Oliveira @DOC9
* Leandro Cruz @Dogma
* Luciano Linhares Martins @SAJ ADV
* Roberto Ugolini @BIPBOP
* Victor Rizzo @e-Xyon

## Atividades do grupo
* Padrão de troca de dados de Processos
* Formato de troca de dados


## Próximas atividades
* Padronização da troca de documentos
* Padronização da autorização e autenticação
* Tabela de apoio de envolvimento em um processo
* Tabela de apoio de orgãos, foros, comarcas e varas
    * Estruturar os dados fornecidos pelo CNJ: https://www.cnj.jus.br/programas-e-acoes/numeracao-unica/documentos/
* Disponibilização das tabelas em um Webservice

## FAQ
* Porque o formato de troca de dados escolhidos foi o JSON? 
    * A decisão foi baseada em critérios, com os respectivos pesos. 
    * Acesso a matriz de decisão: https://docs.google.com/spreadsheets/d/18d0TexNi5tsoRWMZr3Q2F8Vv_KMppcuFbjl0JCK6KtU/edit?usp=sharing
* Como posso fazer o parsing dos dados?
    * Vamos disponibilizar JSON Schema do padrão.
* Qual é o formato de data?
    * O formato de data é AAAA-MM-DD HH:MM:SS-Z da RFC 822 time zone, exemplo: 2020-10-01T12:10:12+03:00
    * Data e hora serão transmitidos no mesmo campo
* Qual é o formato de números?
    * Formato americano com separação por ponto (.) de decimais, exemplo:  1000.00
* Qual é o Charset adotado?
    * UTF-8

