# Plano de Testes — Saucedemo

Plano de testes manuais funcionais aplicado ao Saucedemo (saucedemo.com), um site de e-commerce de prática usado para desenvolvimento de habilidades em QA.

## Objetivo
Validar os principais fluxos do sistema: login, catálogo de produtos, carrinho e checkout, identificando falhas de comportamento.

## Escopo
15 casos de teste funcionais, cobrindo:
- Autenticação (login válido, inválido, bloqueado, campos vazios)
- Catálogo (ordenação de produtos, navegação)
- Carrinho (adicionar, remover, visualizar vazio)
- Checkout (dados válidos, campo obrigatório vazio, finalização)
- Logout

## Resultado
**15/15 casos executados — 15 aprovados, com 1 comportamento inconsistente identificado.**

## Falha encontrada
**Caso 10 — Iniciar checkout sem produtos no carrinho**
O sistema deveria impedir ou alertar o usuário ao tentar iniciar o checkout com o carrinho vazio. No entanto, o fluxo avança normalmente para a etapa de checkout mesmo sem nenhum item selecionado, permitindo prosseguir sem produtos.

Evidência: `evidencias/teste-10-checkout-vazio.png`

## Arquivos
- `Plano_de_Testes_Saucedemo.xlsx` — planilha completa com os 15 casos, passos, resultado esperado, resultado obtido e status
- `evidencias/` — prints das evidências coletadas

## Ferramentas utilizadas
Testes manuais, Google Sheets/Excel para documentação

## Autora
Cauane Silva — [LinkedIn](https://br.linkedin.com/in/cauane-silva-a00357325)
