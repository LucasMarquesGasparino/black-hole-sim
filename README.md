# Black Hole Sim

Simulação visual de buraco negro em página web única (`index.html`), 100% offline.
Um canvas em tela cheia renderiza o buraco negro com disco de acreção e brilho
Doppler, com vinheta cinematográfica e painel de controle (HUD).

## Como abrir

Basta abrir o arquivo no navegador — não precisa de servidor nem internet:

```sh
cd ~/projects/black-hole-sim
python3 -m http.server 8080
# acesse http://localhost:8080
```

Ou toque direto no `index.html` em qualquer navegador do celular.

## Controles (painel HUD)

- **Massa visual** — tamanho do horizonte de eventos / lente gravitacional.
- **Spin** — rotação do buraco negro (arrasta o disco e deforma a imagem).
- **Disco de acreção** — disco luminoso com brilho Doppler (um lado mais
  brilhante, como nas fotos reais de buracos negros).

## Como funciona

- Renderização em `<canvas>` com WebGL/shaders embutidos no próprio HTML.
- Tema escuro, sem dependências externas (sem Three.js, sem CDN).
- Arquivo único: fácil de publicar, incorporar ou abrir offline.

## Estrutura

```
black-hole-sim/
└── index.html   # tudo: cena, shaders, HUD e estilos
```
