# Desdobra

Ferramenta HTML local para desdobramento de apostas de futebol (resultado final 1X2).

## Como usar

Abra o arquivo `desdobramento.html` no navegador (duplo clique ou sirva a pasta com qualquer servidor estático).

1. Adicione os jogos (casa x fora) manualmente **ou** busque pela APIfootball
2. Em cada jogo, marque **1 / X / 2** e/ou **dupla chance (1X / 12 / X2)** com as odds
3. O sistema classifica cada odd (super favorito, favorito forte, etc.)
4. Escolha o modo:
   - **Completo** — produto de todas as opções marcadas
   - **Âncora + Triplas** — 1 fixa (pode ser dupla chance) + desdobro curto
5. Atalhos por jogo: **Só 1X / Só X2 / Só 12** e **Limpar 1X2**
6. No modo âncora, a faixa ideal 1X2 é **1.50–1.85**; em dupla chance ~**1.25–1.55**
7. O painel mostra se cada bilhete sozinho cobre o stake do pacote
8. Copie os bilhetes ou exporte CSV

## Odds via The Odds API

1. Crie uma chave grátis em https://the-odds-api.com/
2. Cole no painel **Buscar odds (The Odds API)**
3. Escolha a liga (ex.: Brasil Série A) e região das casas (EU/UK)
4. **Buscar jogos** → filtre pelo time → **Importar odds**
5. O Desdobra preenche `1/X/2` e, se marcado, busca `1X/12/X2`

A chave fica apenas no `localStorage` do navegador.

## Histórico / conferência

1. Monte o desdobro e clique em **Salvar pacote**
2. Depois do jogo, marque cada bilhete como **Green** ou **Red**
3. O painel mostra apostado, retorno, lucro e **ROI** (só pacotes já liquidados)
4. Exporte o histórico em CSV quando quiser analisar fora
