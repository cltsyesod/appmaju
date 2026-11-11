# Marmitas da Mãe — Preço Final V7

Aplicativo web de página única para calcular o preço final de venda de marmitas. O arquivo `index.html` é uma cópia integral de `marmitas_da_ma_v7_PRECO_FINAL.html`, encontrado em Downloads.

## Como usar

Abra `index.html` no navegador. Escolha o tamanho, selecione os ingredientes e ajuste a quantidade. O preço final do pedido aparece na tela. Em **Ajustar preços**, é possível alterar custos, porções, embalagem, gás/trabalho, reserva de segurança e lucro.

As configurações ficam no `localStorage` deste navegador. Use **Salvar cópia** para baixar um JSON de segurança e **Carregar cópia** para restaurá-lo. Esses dados não são incluídos no repositório nem sincronizados entre dispositivos.

## Cálculo da V7

Para ingredientes em quilos: `custo = preço por kg × gramas / 1000`. Para ovos: `custo = preço por unidade × quantidade de ovos`. Se a porção não foi definida, a V7 distribui o peso do tamanho escolhido entre os ingredientes selecionados por pesos de grupo e estima a quantidade de ovos.

`preço por marmita = [custo dos ingredientes × (1 + segurança/100) + embalagem + gás/trabalho] × (1 + lucro/100)`

`preço final do pedido = preço por marmita × quantidade`

Alguns custos e despesas iniciais são estimativas. Confirme custos, rendimento e porções antes de usar o preço comercialmente. A entrega não entra no cálculo.

## Publicação

O projeto é estático e não precisa de dependências nem build. Para usar GitHub Pages, publique a raiz da branch escolhida; o `index.html` será a página inicial.
