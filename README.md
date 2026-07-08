# Impacto e Influência dos Filmes e Séries a Nível Cultural

Trabalho prático desenvolvido para a unidade curricular de **Engenharia de Dados para Suporte à Tomada de Decisão (EDSTD)**.

_Nota: Este repositório é uma cópia para fins de portfólio pessoal._

## Descrição

Projeto de Data Lakehouse que implementa uma arquitetura Medallion (Bronze/Silver/Gold) utilizando Apache Spark e HDFS para analisar o impacto cultural e comercial de filmes e séries. O projeto integra dados heterogêneos provenientes de serviços de streaming, retorno financeiro e adaptações literárias, visando correlacionar a aclamação da crítica, a popularidade e o comportamento do consumidor.

## Autores

- Sérgio Paulo Vieira Carvalho [@serginho355](https://github.com/serginho355)
- Pedro Manuel Mendes Neves [@pedro2516](https://github.com/pedro2516)
- Filipa Mendes de Castro Pinto [@filipamcp](https://github.com/filipamcp)
- Rodrigo Santiago Faria Fonseca Abreu [@Rabreu01](https://github.com/Rabreu01)
- Maria Vitória Veloso Costa Coutinho Alves

## Arquitetura

| Camada | Descrição                                                                                                           |
| ------ | ------------------------------------------------------------------------------------------------------------------- |
| Bronze | Ingestão e armazenamento dos dados brutos extraídos do Kaggle e Wikidata em formato original dentro do HDFS.        |
| Silver | Limpeza, deduplicação, normalização de esquemas e cruzamento de dados (ex.: mapeamento de livros para IDs do IMDb). |
| Gold   | Criação de tabelas de factos e dimensões otimizadas para responder às questões analíticas e de negócio.             |

## Fontes de Dados Integradas

| Domínio          | Fontes de Dados Utilizadas                                                     |                                                    
| ---------------- | ------------------------------------------------------------------------------ |
| Cinema e Prémios | Óscares, Retorno Financeiro, IMDb.                                             |
| Streaming        | Catálogos e créditos da Netflix e da Amazon Prime Video.                       |
| Literatura       | Adaptações literárias                                                          |
| Música           | Preferências globais de música, vencedores dos Grammys e bandas sonoras.       |

## Tecnologias Principais

- Orquestração e Processamento: Apache Spark 
- Armazenamento Distribuído: Hadoop Distributed File System (HDFS)
- Ambiente de Trabalho: Jupyter Notebooks
- Visualização de Dados: Tableau
