# Stremio PS4 (nativo) — como usar

Base: port do starsitaxyz (GPL-3.0) sobre o port do PS5 de Sp9nky. Veja README.md e THIRD_PARTY.md.

## Compilar (sem instalar nada no PC)
1. Suba todo este conteúdo para o seu repositório no GitHub (branch `main` ou `nativo`).
2. Aba **Actions** → **Build PS4 PKG** → **Run workflow**. Leva até ~90 min.
3. Quando terminar, baixe o artifact **stremio-ps4** (contém o .pkg).
4. Instale o .pkg no PS4 com o instalador de homebrew de sempre.

## Se o vídeo não tocar
Copie `/data/stremio/log.txt` do PS4 e envie. Procure as linhas "ps4 hwdec" e "player: software video decoding".

## Dicas
- Prefira streams H.264 em 1080p/720p; 4K não roda.
- Se o build falhar, baixe `build.log` e `compiler.log` nos artifacts.
