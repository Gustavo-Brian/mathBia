# Supabase

## 1. Criar a tabela

No painel do Supabase, abra `SQL Editor` e rode o arquivo:

`supabase-schema.sql`

Ele cria a tabela `user_progress` com Row Level Security. Cada usuario autenticado so consegue ler e gravar a propria linha de progresso.

## 2. Conferir as credenciais publicas

O arquivo `supabase-config.js` ja esta preenchido com a URL e a chave publica do projeto:

```js
window.SUPABASE_CONFIG = {
  url: 'https://hkkkbqclfqdyexqwvnrd.supabase.co',
  anonKey: 'sb_publishable_tKFyTHqWg2GdW2C6gnUsuA_2XOMVd4n',
  table: 'user_progress'
};
```

Use somente a chave publica `anon`/`publishable` no frontend. Nunca coloque a `service_role` nem a string direta do Postgres no Vercel, no GitHub ou em qualquer arquivo publico.

## 3. Ativar conta simples

A interface mostra apenas `Nome` e `Senha`. Por baixo, o app transforma o nome em um identificador interno no formato `nome@mathbia.local`, porque o Supabase Auth trabalha com e-mail/senha.

No painel do Supabase:

1. Va em `Authentication > Providers`.
2. Deixe `Email` ativo.
3. Deixe `Confirm email` desativado para este projeto de teste com pessoas conhecidas.
4. Mantenha senha minima de 6 caracteres, que e o minimo esperado pelo Supabase.

Se `Confirm email` ficar ativado, a conta pode ser criada sem entrar automaticamente, porque o e-mail interno nao e uma caixa real.

## 4. Configurar URLs do Auth

Em `Authentication > URL Configuration`, use a URL real do deploy.

Durante testes locais:

- Site URL: `http://localhost:4173/`
- Redirect URLs: `http://localhost:4173/`

Depois do deploy no Vercel, troque/adicione:

- Site URL: `https://SEU-PROJETO.vercel.app/`
- Redirect URLs: `https://SEU-PROJETO.vercel.app/`

Se o Vercel gerar uma URL diferente, use exatamente a URL mostrada no dashboard.

## 5. Testar

Abra o site, crie uma conta com nome e senha, resolva algumas questoes e confira no Supabase se a tabela `user_progress` recebeu uma linha para esse usuario.
