# Visão Geral da Arquitetura

O SIG foi projetado com foco em **clareza de dados, rastreabilidade e evolução segura**.

A arquitetura adota os seguintes princípios:

- Uma **entidade raiz** representa uma linha da planilha
- Cada bloco da planilha vira uma **tabela própria**
- Relacionamentos 1:1 preservam a estrutura original
- Campos permanecem flexíveis na fase inicial (Text / Date / Decimal)

## Componentes principais

- Banco de dados: PostgreSQL
- Backend: Django
- Admin: Django Admin (validação estrutural)
- Documentação: MkDocs Material

## Estratégia de modelagem

A planilha original possui mais de 90 colunas.  
Ao invés de uma tabela monolítica, os dados foram organizados em:

- uma tabela central (`sig_registro`)
- tabelas auxiliares por etapa do processo (1:1)
- tabelas independentes para abas auxiliares

Isso reduz acoplamento e facilita manutenção.
