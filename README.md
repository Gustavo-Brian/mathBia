# MathBia

Plataforma estatica de estudos de equacoes, com entrada simples por nome, teoria guiada, pratica interativa, estatisticas por usuario e sincronizacao via Supabase. Uma nova aba sempre inicia na tela de cadastro/login; depois de entrar, a navegacao entre paginas continua liberada naquela aba.

## Arquivos principais

- `index.html`: entrada da plataforma.
- `01-...html` a `22-...html`: conteudos e simulados.
- `supabase-config.js`: URL e chave publica do Supabase.
- `vendor/supabase-js.js`: copia local da biblioteca publica do Supabase, usada quando o CDN nao carregar.
- `supabase-schema.sql`: tabela e policies RLS para progresso por usuario.
- `supabase-instrucoes.md`: passo a passo de configuracao.

## Deploy com Vercel

1. Importe o repositorio `Gustavo-Brian/math` no Vercel.
2. Use `Other` como preset.
3. Mantenha `Root Directory` como `./`.
4. Nao precisa configurar build command nem output directory.
5. Clique em `Deploy`.

Como o projeto e estatico, o Vercel publica os arquivos HTML diretamente.

## Supabase Auth

No Supabase, em `Authentication > Providers`, deixe `Email` ativo e desative `Confirm email`, porque a tela usa entrada simples apenas com `Nome`.

Em `Authentication > URL Configuration`, configure:

- Site URL: a URL final do Vercel, por exemplo `https://math-bia.vercel.app/`.
- Redirect URLs: a mesma URL do Vercel e URLs locais usadas em teste, como `http://localhost:4173/`.

Use sempre a chave publica `anon`/`publishable` no frontend. Nunca use `service_role` nem string direta do Postgres em arquivos do site.
