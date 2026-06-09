# Supabase

## 1. Criar a tabela

No painel do Supabase, abra SQL Editor e rode o arquivo:

`supabase-schema.sql`

Ele cria a tabela `user_progress` com Row Level Security. Cada usuario autenticado so consegue ler e gravar a propria linha.

## 2. Conferir as credenciais

O arquivo `supabase-config.js` ja esta preenchido com a URL e a chave publica do projeto:

```js
window.SUPABASE_CONFIG = {
  url: 'https://hkkkbqclfqdyexqwvnrd.supabase.co',
  anonKey: 'sb_publishable_tKFyTHqWg2GdW2C6gnUsuA_2XOMVd4n',
  table: 'user_progress'
};
```

Use a chave `anon public`, nunca a `service_role`.

## 3. Ativar login por e-mail

No Supabase, confira em Authentication que o login por e-mail/senha esta ativo.

## 4. Configurar URLs do Auth

Em Authentication > URL Configuration, use:

- Site URL: `https://gustavo-brian.github.io/mathBia/`
- Redirect URLs: `https://gustavo-brian.github.io/mathBia/` e `http://localhost:4173/`

Depois disso, abra o material, va em Configuracoes > Conta e entre/crie uma conta.
