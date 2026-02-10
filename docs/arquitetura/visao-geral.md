# Visão geral

O SIG é um sistema (Django + PostgreSQL) derivado da planilha SIG_Para_Sistema.xlsx.

Objetivo inicial:

- Replicar a planilha no banco de dados com fidelidade (estrutura e campos)
- Preservar vínculos entre informações por registro

Estratégia adotada:

- Um registro raiz por linha da planilha (UUID)
- Blocos da planilha separados em tabelas 1:1 (OneToOne) para evitar uma tabela monolítica
- Abas auxiliares como tabelas próprias (ex.: Controle ADM, Implantação, Materiais)
