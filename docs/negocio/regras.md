# Regras de negócio (baseadas na planilha)

## Conceito de previsto x realizado

A planilha trabalha com marcos em pares:

- `prev_*`: data planejada
- `real_*`: data realizada

Regras:

- Se `real_*` existe, a etapa foi concluída.
- Se só `prev_*` existe, a etapa está planejada.
- Se nenhum existe, a etapa ainda não foi iniciada/definida.

## Status

O status atual do registro fica em `sig_andamento.status`.
Na fase inicial, o campo é texto (fiel à planilha). Em fases futuras, recomenda-se padronizar (enum).

## Financeiro

Campos principais:

- compra prevista vs compra real
- valor de venda

Fórmulas e indicadores serão implementados depois (híbrido: Python + SQL).
