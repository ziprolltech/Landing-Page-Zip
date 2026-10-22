# Landing page ZipRoll

Site de uma página da ZipRoll, plataforma de distribuição automatizada de holerites.
O design (layout, tipografia Oswald + Space Grotesk, hero em WebGL com mapa de
profundidade, transições em xadrez, linha do tempo, placa de estatísticas e rodapé)
é o mesmo do projeto `ziprolltech/Landing-Page_Neymar`, com a paleta da marca
(navy `#1c1e2c`, creme `#fcf5e4`, dourado `#c4a96a`), a onça do logotipo e o
conteúdo da ZipRoll.

## Rodar

Os módulos ES e as texturas precisam de um servidor (não abre direto pelo `file://`):

```bash
python -m http.server 8080
# abra http://localhost:8080
```

Three.js e Lenis vêm do jsDelivr; o restante está em `assets/`.

## Estrutura

```
index.html          página inteira (CSS + JS inline)
assets/brand/       logo, símbolo e wordmark originais da ZipRoll
assets/hero/        onça: diffuse, alpha, profundidade, normal e overlay do hover
assets/timeline/    as cinco telas de "Como funciona" (passo-01 a passo-05)
assets/paddock/     onça dourada da seção de preços
assets/footer/      onça creme e máscara do wordmark do rodapé
assets/ui/          wordmark navy, máscara do loader, ícones de fluxo e documento
assets/remote/      ruído do shader, linhas de fundo, botão de play, ícones de preços
```

## Seções e âncoras do menu

| Menu            | Âncora      | Conteúdo                                   |
|-----------------|-------------|--------------------------------------------|
| Como funciona   | `#timeline` | cinco passos, do PDF ao celular            |
| Funcionalidades | `#season`   | mapa em meio-tom, resumo e placa ZR / RH   |
| Preços          | `#paddock`  | Starter, Pro, Enterprise e teste grátis    |
| Contato         | `#footer`   | chamada final, links e rodapé              |

Nomes, matrículas e valores exibidos são exemplos.
