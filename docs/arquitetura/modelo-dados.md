# Modelo de dados

## Entidade raiz

A tabela raiz é `sig_registro`. Cada linha representa um cliente/OS/serial e possui um UUID.

## Blocos 1:1

A aba principal (Base_Dados) foi quebrada em tabelas 1:1 por seção da planilha, todas vinculadas por `sig_registro.id`.

## Abas auxiliares

- Controle ADM: 1:1 com o registro (mesmo UUID)
- Implantação: tabela independente (vínculo será definido na fase de importação)
- Materiais: catálogo auxiliar
