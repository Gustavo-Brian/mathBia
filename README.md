# MathBia

Plataforma estatica de estudos de equacoes, com progresso local e sincronizacao por usuario via Supabase.

## Arquivos principais

- `index.html`: entrada da plataforma.
- `01-...html` a `22-...html`: conteudos e simulados.
- `supabase-config.js`: URL e chave publica do Supabase.
- `vendor/supabase-js.js`: copia local da biblioteca publica do Supabase, usada quando o CDN nao carregar.
- `supabase-schema.sql`: tabela e policies RLS para progresso por usuario.
- `supabase-instrucoes.md`: passo a passo de configuracao.

## Deploy com GitHub Pages

1. Suba estes arquivos para a branch `main`.
2. No GitHub, abra `Settings > Pages`.
3. Em `Build and deployment`, escolha `Deploy from a branch`.
4. Selecione `main` e pasta `/root`.
5. Acesse `https://gustavo-brian.github.io/mathBia/`.

## Supabase Auth

No Supabase, em `Authentication > URL Configuration`, configure:

- Site URL: `https://gustavo-brian.github.io/mathBia/`.
- Redirect URLs: `https://gustavo-brian.github.io/mathBia/` e URLs locais usadas em teste, como `http://localhost:4173/`.

Use sempre a chave publica `anon`/`publishable` no frontend. Nunca use `service_role` nem string direta do Postgres em arquivos do site.
