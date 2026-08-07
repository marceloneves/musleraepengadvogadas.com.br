# musleraepengadvogadas.com.br

Site institucional do **Muslera & Peng Advogadas Associadas** — Florianópolis/SC.

Site estático, sem build. O conteúdo fica na raiz do repositório, então qualquer
host que sirva `index.html` de diretório (Vercel, Netlify, GitHub Pages, nginx,
Apache) publica direto, sem configuração.

## Rodar localmente

```bash
python3 -m http.server 4321
# http://127.0.0.1:4321
```

## Estrutura

- uma pasta por URL — `/sobre-nos/`, `/servicos/direito-de-familia/`, `/equipe/pricila-moreira-peng/`
- `wp-content/uploads/brand/` — logotipo, favicons, fotos do escritório e `brand.css`
- `wp-content/themes/` e `wp-content/plugins/` — CSS e JS do tema

Os ajustes de identidade (paleta, logotipo, tipografia, correções de layout e
acessibilidade) ficam concentrados em `wp-content/uploads/brand/brand.css`,
carregado por último no `<head>` de todas as páginas.
