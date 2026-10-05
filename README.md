# rpa-automacao-estoque-python
Script de automação de processos e relatórios para auto peças
# Automação de Monitoramento e Controle de Estoque Operacional (RPA)

## Visão Geral do Projeto
Este repositório contém a implementação de uma Automação de Processos Robóticos (RPA) desenvolvida em Python e SQL. O objetivo principal do projeto é automatizar a auditoria de níveis de inventário em sistemas de gestão de autopeças e e-commerce, identificando inconformidades de estoque e gerando relatórios operacionais para tomada de decisão ágil pela equipe de suprimentos.

## Contexto e Regra de Negócio
Em operações logísticas e de e-commerce automotivo, a verificação manual de saldo de produtos em relação ao estoque mínimo é sujeita a falhas humanas e atrasos operacionais. 

O robô executa o seguinte fluxo de trabalho:
1. Conecta-se ao banco de dados relacional e executa a extração dos dados cadastrais e de inventário.
2. Aplica a regra de negócio para identificar produtos cuja quantidade em estoque é inferior ao limite de segurança estabelecido.
3. Tratamento, formatação e validação dos dados retornados.
4. Exportação automática de um relatório consolidado em formato CSV contendo os itens críticos para reposição.

## Tecnologias e Ferramentas Utilizadas
- Linguagem de Programação: Python 3
- Banco de Dados Relacional: SQL (SQLite)
- Processamento e Manipulação de Dados: Pandas
- Bibliotecas Nativas: sqlite3, datetime

## Arquitetura do Código
- init_db(): Função responsável pela inicialização e estruturação do banco de dados relacional e inserção de dados de validação.
- executar_bot_rpa(): Módulo principal de automação que executa as consultas SQL filtradas, processa a massa de dados e exporta os relatórios com data stamp.


### Pré-requisitos
- Python 3.8 ou superior instalado.
- Biblioteca Pandas instalada.

### Instalação de Dependências
```bash
pip install pandas
