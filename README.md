# musleraepengadvogadas.com.br

Site institucional do **Muslera & Peng Advogadas Associadas** — Florianópolis/SC.

Site estático. O conteúdo publicado fica em [`site/`](site/); qualquer servidor
que entregue `index.html` de diretório (nginx, Apache, Vercel, GitHub Pages)
serve a pasta como está.

## Rodar localmente

```bash
cd site
python3 -m http.server 4321
# http://127.0.0.1:4321
```

## Estrutura

- `site/` — páginas HTML, uma pasta por URL (`/sobre-nos/`, `/servicos/direito-de-familia/`, …)
- `site/wp-content/uploads/brand/` — logotipo, favicons, fotos do escritório e `brand.css`
- `site/wp-content/themes/` e `site/wp-content/plugins/` — CSS e JS do tema

Os ajustes de identidade (paleta, logotipo, tipografia, correções de layout e
acessibilidade) ficam concentrados em `site/wp-content/uploads/brand/brand.css`,
carregado por último no `<head>` de todas as páginas.
