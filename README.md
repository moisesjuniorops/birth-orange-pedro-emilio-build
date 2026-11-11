# Doze Anos de Orange

Página de aniversário para Pedro Emílio. Site estático, sem build: abre direto no GitHub Pages.

## Estrutura

```
index.html          página inteira (HTML, CSS e JS)
assets/img/         fotos e o sol da Orange (PNG sem fundo)
.nojekyll           pede ao GitHub Pages para servir os arquivos como estão
```

## Publicar no GitHub Pages

1. Crie um repositório novo no GitHub, por exemplo `pedro-12-anos`.
2. Na pasta do projeto:

   ```bash
   git init -b main
   git add .
   git commit -m "feat: add birthday page"
   git remote add origin git@github.com:SEU-USUARIO/pedro-12-anos.git
   git push -u origin main
   ```

3. No repositório, abra **Settings → Pages**. Em **Build and deployment**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
4. Em cerca de um minuto, a página fica em `https://SEU-USUARIO.github.io/pedro-12-anos/`.

## Antes de enviar

- Repositório público deixa a página aberta para quem tiver o link, inclusive a foto da Alba. A página já pede aos buscadores para não indexar (`noindex`), mas isso não a protege. Use um nome de repositório difícil de adivinhar. Páginas de repositório privado exigem um plano pago do GitHub.
- Para o QR code ou a etiqueta NFC, defina o endereço final antes de imprimir ou gravar.

## Como editar

- **Nomes, legendas e fotos das obras:** objeto `ITENS` no final do `index.html`.
- **Ordem e tamanho dos prédios:** lista `LAY`, logo abaixo.
- **Textos de "Na obra" e "Em casa":** seção 02 do `index.html`.
- **Trocar uma foto:** substitua o arquivo em `assets/img/` mantendo o nome. Prefira JPG com até 1200 px de largura.
