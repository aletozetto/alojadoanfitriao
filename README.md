# Site ALoja do Anfitrião — Sistema ANFITRIÃO™

Site institucional e comercial estático (HTML + Tailwind via CDN). Sem build step.

## Estrutura

```
index.html                      → /  (home institucional)
anfitr-ia.html                  → /anfitr-ia  (pilar de automação)
anfitr-ia-limpeza.html          → /anfitr-ia/limpeza
anfitr-ia-atendimento.html      → /anfitr-ia/atendimento
anfitr-ia-jornadahospede.html   → /anfitr-ia/jornadahospede
mentoria.html                   → /mentoria
gestao-otas.html                → /gestao-otas
sobre.html                      → /sobre
img/                            → todas as imagens
_redirects                      → URLs limpas + redirects 301 das URLs antigas
netlify.toml                    → config sem build + cache headers
sitemap.xml / robots.txt        → SEO
```

## Deploy no Netlify

1. **Backup**: baixe o projeto atual antes de substituir.
2. Suba TODOS estes arquivos para a raiz do repositório GitHub conectado ao Netlify
   (apague os arquivos antigos do projeto Vite/React antes).
3. O Netlify detecta o push e publica automaticamente.
4. `netlify.toml` desativa o build — não roda `npm run build`.

## Pós-deploy

- [ ] Conferir preview do WhatsApp (OG image nova)
- [ ] Reenviar sitemap no Google Search Console
- [ ] Validar URLs antigas redirecionando (ex: /ecossistema → /anfitr-ia)
- [ ] Testar todos os botões de CTA (devem abrir WhatsApp 5512991638478 com tag de lead)

## Placeholders a substituir depois

- `/anfitr-ia/atendimento` → bloco de conversa real do Chatwoot (hoje placeholder)
- Depoimentos reais de Victor/DaCali e Liz/ZanaLofts7 (P0 no backlog)

## CTAs por página (tag de lead para a IAra)

| Página | Tag |
|---|---|
| Home | `[LEAD-HOME]` |
| /anfitr-ia | `[LEAD-ANFITRIA]` |
| /anfitr-ia/limpeza | `[LEAD-LIMPEZA]` |
| /anfitr-ia/atendimento | `[LEAD-ATENDIMENTO]` |
| /anfitr-ia/jornadahospede | `[LEAD-JORNADA]` |
| /mentoria | `[LEAD-MENTORIA]` |
| /gestao-otas | `[LEAD-GESTAO-OTAS]` |
| /sobre | `[LEAD-SOBRE]` |
