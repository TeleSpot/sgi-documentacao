# Relacionamento entre Tabelas

## Visão geral

- `sig_registro` é a tabela central
- Todas as tabelas de bloco dependem dela
- Relacionamento: 1 registro → 0 ou 1 bloco

## Tabelas dependentes (1:1)

- sig_andamento
- sig_equipe_campo
- sig_equipamento
- sig_financeiro
- sig_viabilidade_inicial
- sig_vistoria_inicial
- sig_relatorio_vistoria
- sig_pre_projeto
- sig_proposta_comercial
- sig_projeto_executivo
- sig_instalacao_equipamento
- sig_relatorio_instalacao
- sig_aprovacao_concessionaria
- sig_comissionamento_ativacao
- sig_cancelamento
- sig_obs
- sig_controle_adm

## Tabelas independentes

- sig_implantacao
- sig_material

Essas tabelas serão associadas ao fluxo principal em fases futuras.
