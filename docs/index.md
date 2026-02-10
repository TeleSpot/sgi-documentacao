# SIG – Sistema de Gestão Integrada

Esta documentação descreve o **SIG**, um sistema web desenvolvido para substituir e evoluir uma planilha operacional complexa, atualmente utilizada para controle de clientes, etapas de execução, prazos, custos e resultados financeiros.

O sistema foi inicialmente modelado para **replicar fielmente a planilha**, preservando:

- estrutura dos dados
- dependências entre colunas
- lógica de previsto × realizado
- regras implícitas usadas no dia a dia

A partir dessa base, o SIG evoluirá para:

- validações automáticas
- alertas de prazo
- indicadores financeiros
- relatórios consolidados
- integração com outros sistemas

## Escopo atual

- Modelagem de dados (PostgreSQL)
- Backend em Django
- Documentação de regras de negócio
- Base preparada para importação do XLSX

## Escopo futuro

- Importação assistida da planilha
- API e frontend
- Normalização de dados e enums
- Automação de cálculos e alertas
