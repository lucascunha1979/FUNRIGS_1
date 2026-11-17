# Painel FUNRIGS — Fundo do Plano Rio Grande

Painel público sobre os recursos recebidos e a execução da despesa do FUNRIGS, feito a partir das planilhas do Portal da Transparência do RS.

## O que tem aqui

| Caminho | O que é |
|---|---|
| `painel_funrigs.ipynb` | Notebook (Google Colab) que lê as planilhas, confere, calcula os índices e gera o painel |
| `dados/` | Planilhas `.xlsx` exportadas do portal (uma de execução e uma de recursos recebidos por mês) |
| `docs/index.html` | O painel. É este arquivo que o GitHub Pages publica |
| `saidas/` | Cópia datada do painel e tabela CSV com todos os indicadores e notas |

## Primeira publicação

1. Crie um repositório **público** no GitHub e envie estas pastas (botão *Add file → Upload files*; arraste as pastas inteiras).
2. Em *Settings → Pages*, escolha *Deploy from a branch*, ramo `main`, pasta `/docs`, e salve.
3. No notebook, na célula 1, preencha `GITHUB_USUARIO` e `GITHUB_REPOSITORIO`.

## Atualização mensal

1. Baixe do portal as duas planilhas novas.
2. Envie as duas para `dados/`. Não apague as antigas: o notebook usa a mais recente de cada tipo (pela maior data dentro da planilha).
3. Abra `painel_funrigs.ipynb` no Colab e execute tudo.
4. O Colab baixa `index.html` e o CSV dos índices. Envie o `index.html` para `docs/`, substituindo o anterior. Guarde a cópia datada em `saidas/` se quiser manter o histórico.

Sem GitHub configurado, o notebook pede o upload das duas planilhas no próprio Colab.

## Regras de cálculo

Estão explicadas em linguagem simples na aba **Notas e método** do painel. Os parâmetros (janela de maturação, mínimos para receber nota, pesos) ficam na célula 1 do notebook.
