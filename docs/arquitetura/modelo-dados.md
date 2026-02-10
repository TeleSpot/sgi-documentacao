# Modelo de Dados

## Entidade Raiz

A tabela `sig_registro` representa **uma linha da aba principal da planilha**.

Ela contém:

- identificação do cliente
- número da OS / serial
- UUID único que vincula todas as demais tabelas

## Blocos 1:1

Cada bloco da planilha (viabilidade, vistoria, financeiro, etc.) foi convertido em uma tabela com relacionamento **OneToOne** com `sig_registro`.

Características:

- mesma chave primária (UUID)
- dependência direta do registro raiz
- dados opcionais na fase inicial

## Abas auxiliares

Algumas abas da planilha não possuem vínculo direto por ID e foram modeladas separadamente:

- Controle ADM (1:1 com registro)
- Implantação (vínculo definido futuramente)
- Materiais (catálogo)
