# Prompt para o Codex — Plataforma completa de Equações em HTML autônomo

Você deve criar uma plataforma completa de estudo de álgebra e equações com base no arquivo:

```text
guia_completo_equacoes_para_codex.md
```

Leia o guia inteiro antes de começar. Ele define a ordem dos conteúdos, os tópicos teóricos, os tipos de exercícios e os requisitos pedagógicos.

O objetivo não é criar uma demonstração simples. O resultado deve ser uma coleção completa de páginas HTML funcionais, bem estilizadas, didáticas, responsivas e interativas.

---

# Regra principal

Todos os arquivos devem ser páginas HTML autônomas.

Cada arquivo `.html` deve conter dentro dele:

- Todo o HTML;
- Todo o CSS em uma tag `<style>`;
- Todo o JavaScript em uma tag `<script>`;
- Todos os ícones como SVG inline, CSS ou caracteres Unicode;
- Todo o banco de questões necessário para aquela página;
- Todos os textos, exemplos, dicas e resoluções.

Não criar arquivos separados de CSS ou JavaScript.

Não usar:

- React;
- Vue;
- Angular;
- Bootstrap;
- Tailwind via CDN;
- jQuery;
- Bibliotecas externas;
- Fontes externas;
- Imagens externas;
- APIs;
- `eval`;
- Dependências que exijam instalação;
- Processo de build;
- Servidor obrigatório.

As páginas devem funcionar ao serem abertas diretamente no navegador por meio de `file://`.

---

# Objetivo do projeto

Criar uma plataforma de aprendizagem que permita ao estudante:

- Aprender teoria;
- Acompanhar exemplos resolvidos;
- Praticar exercícios;
- Receber dicas progressivas;
- Ver resoluções passo a passo;
- Registrar acertos e erros;
- Revisar questões erradas;
- Acompanhar o próprio progresso;
- Fazer simulados;
- Navegar por uma trilha organizada;
- Usar tudo no computador ou celular;
- Estudar mesmo sem conexão com a internet.

---

# Idioma

Todo o projeto deve ser escrito em português do Brasil.

Isso inclui:

- Interface;
- Botões;
- Mensagens;
- Explicações;
- Dicas;
- Resoluções;
- Atributos de acessibilidade;
- Exemplos;
- Comentários importantes do código.

---

# Arquivos que devem ser criados

Criar a seguinte estrutura:

```text
/
├── index.html
├── 01-fundamentos-aritmeticos.html
├── 02-expressoes-algebricas.html
├── 03-termos-semelhantes.html
├── 04-propriedade-distributiva.html
├── 05-equacoes-primeiro-grau.html
├── 06-problemas-primeiro-grau.html
├── 07-inequacoes-primeiro-grau.html
├── 08-sistemas-primeiro-grau.html
├── 09-funcao-primeiro-grau.html
├── 10-produtos-notaveis.html
├── 11-fatoracao.html
├── 12-equacoes-segundo-grau.html
├── 13-funcao-segundo-grau.html
├── 14-inequacoes-segundo-grau.html
├── 15-equacoes-fracionarias.html
├── 16-equacoes-irracionais.html
├── 17-modulo.html
├── 18-equacoes-exponenciais.html
├── 19-logaritmos.html
├── 20-sistemas-avancados.html
├── 21-revisao-geral.html
└── 22-simulados.html
```

Cada página de conteúdo deve reunir teoria e prática no mesmo HTML, por meio de abas ou seções internas.

Não gerar arquivos vazios, incompletos ou com textos como:

```text
Conteúdo em breve
TODO
Adicionar exercícios depois
Exemplo genérico
```

Todas as páginas devem estar realmente preenchidas.

---

# Organização interna de cada página

Cada módulo deve conter as seguintes áreas:

1. Cabeçalho;
2. Menu de navegação;
3. Trilha de progresso;
4. Título do módulo;
5. Objetivos de aprendizagem;
6. Pré-requisitos;
7. Aba de teoria;
8. Aba de exemplos;
9. Aba de prática;
10. Aba de revisão de erros;
11. Resumo;
12. Navegação para módulo anterior e seguinte;
13. Rodapé;
14. Painel de configurações.

Usar abas acessíveis, com suporte a:

- Clique;
- Teclado;
- `aria-selected`;
- `role="tab"`;
- `role="tabpanel"`.

---

# Página inicial

O arquivo `index.html` deve funcionar como painel principal da plataforma.

Ele deve conter:

## Apresentação

- Nome da plataforma;
- Descrição curta;
- Explicação de como estudar;
- Botão “Continuar de onde parei”;
- Botão “Começar do início”;
- Botão “Revisar meus erros”.

## Trilha completa

Exibir todos os módulos em cartões.

Cada cartão deve mostrar:

- Número;
- Nome;
- Descrição;
- Nível;
- Pré-requisitos;
- Porcentagem concluída;
- Quantidade de questões respondidas;
- Taxa de acerto;
- Estado: não iniciado, em andamento ou concluído;
- Botão para abrir.

## Painel de progresso

Mostrar:

- Progresso geral;
- Total de questões respondidas;
- Total de acertos;
- Total de erros;
- Taxa geral de acerto;
- Melhor sequência de acertos;
- Módulo mais estudado;
- Conteúdo com pior desempenho;
- Data da última sessão;
- Tempo total estimado de estudo.

## Ações

Incluir:

- Limpar progresso;
- Exportar progresso;
- Importar progresso;
- Alternar tema;
- Ativar ou desativar animações;
- Ativar ou desativar sons;
- Modo de alto contraste;
- Aumentar ou reduzir fonte.

A limpeza de progresso deve pedir confirmação.

A exportação deve gerar um arquivo JSON usando JavaScript no navegador.

A importação deve aceitar um arquivo JSON previamente exportado e validar sua estrutura.

---

# Padrão visual

Criar um design moderno, elegante e profissional.

## Aparência

Usar:

- Cartões;
- Bordas suaves;
- Sombras discretas;
- Espaçamento consistente;
- Tipografia do sistema;
- Hierarquia visual clara;
- Ícones em SVG inline;
- Animações discretas;
- Feedback visual de interação.

## Temas

Implementar:

- Tema claro;
- Tema escuro;
- Tema automático baseado no sistema;
- Modo de alto contraste.

Salvar a preferência no `localStorage`.

## Cores

Usar variáveis CSS.

Exemplo de organização:

```css
:root {
  --bg:
  --surface:
  --surface-2:
  --text:
  --muted:
  --primary:
  --primary-hover:
  --success:
  --warning:
  --danger:
  --border:
  --shadow:
  --radius:
}
```

Não espalhar valores de cor sem organização.

## Responsividade

A interface deve funcionar bem em:

- Celulares pequenos;
- Celulares grandes;
- Tablets;
- Notebooks;
- Monitores grandes.

Usar uma coluna em telas pequenas.

Evitar rolagem horizontal, exceto em fórmulas ou tabelas que realmente precisem.

---

# Acessibilidade

Implementar:

- HTML semântico;
- Labels associados aos campos;
- Navegação por teclado;
- Foco visível;
- Contraste adequado;
- `aria-live` para feedback de respostas;
- `aria-expanded` em menus;
- `aria-current` na navegação;
- Botões com nomes claros;
- Textos alternativos quando necessário;
- Suporte a `prefers-reduced-motion`;
- Tamanho mínimo adequado para áreas clicáveis;
- Mensagens que não dependam apenas de cor.

Criar um link “Pular para o conteúdo”.

---

# Conteúdo teórico

Cada módulo deve trazer uma explicação completa baseada no guia.

Não resumir demais.

A teoria deve conter:

- Definição;
- Intuição;
- Regras;
- Vocabulário;
- Fórmulas;
- Passos de resolução;
- Exemplos básicos;
- Exemplos intermediários;
- Exemplos avançados;
- Erros comuns;
- Comparações entre métodos;
- Pequeno resumo final;
- Perguntas rápidas de revisão.

## Fórmulas

Como não serão usadas bibliotecas externas, formatar as fórmulas com:

- HTML semântico;
- `<sup>`;
- `<sub>`;
- Frações construídas com CSS;
- Símbolos Unicode;
- Blocos visuais próprios;
- `aria-label` contendo a leitura da fórmula.

Criar componentes CSS como:

```html
<span class="fraction" aria-label="a sobre b">
  <span class="numerator">a</span>
  <span class="denominator">b</span>
</span>
```

As fórmulas devem permanecer legíveis em telas pequenas.

---

# Exemplos resolvidos

Cada módulo deve conter no mínimo:

- 4 exemplos básicos;
- 4 exemplos intermediários;
- 3 exemplos avançados.

Cada exemplo deve apresentar:

1. Enunciado;
2. Estratégia;
3. Passos numerados;
4. Resultado;
5. Verificação;
6. Observação sobre erro comum.

Criar um botão para mostrar ou esconder a resolução.

Não exibir todas as resoluções automaticamente.

---

# Área de prática

Cada módulo deve ter exercícios interativos.

## Quantidade mínima

Cada página deve possuir um banco com pelo menos:

- 20 questões básicas;
- 20 questões intermediárias;
- 15 questões avançadas.

Total mínimo:

```text
55 questões por módulo
```

Quando o tipo de conteúdo permitir, parte das questões pode ser gerada dinamicamente a partir de modelos matemáticos seguros.

Não usar `eval`.

## Tipos de exercício

Usar uma combinação de:

- Resposta numérica;
- Resposta algébrica curta;
- Múltipla escolha;
- Verdadeiro ou falso;
- Complete os passos;
- Ordene os passos;
- Identifique o erro;
- Associe conceitos;
- Interprete um gráfico;
- Monte a equação;
- Problema contextualizado.

Não usar apenas múltipla escolha.

## Modos de prática

Implementar:

### Prática livre

O estudante escolhe nível e quantidade.

### Sessão rápida

Gerar 5 questões.

### Sessão padrão

Gerar 10 questões.

### Sessão intensiva

Gerar 20 questões.

### Revisão de erros

Usar apenas questões respondidas incorretamente.

### Desafio misto

Misturar tipos e níveis.

---

# Validação de respostas

A validação deve ser segura e tolerante.

Aceitar equivalências como:

```text
0,5
0.5
1/2
```

quando representarem o mesmo valor.

Também aceitar:

```text
x=5
x = 5
5
```

quando o campo pedir o valor de `x`.

## Regras

Criar funções próprias para:

- Normalizar espaços;
- Trocar vírgula decimal por ponto;
- Interpretar frações numéricas simples;
- Comparar números com pequena tolerância;
- Normalizar sinais;
- Verificar listas de soluções;
- Desconsiderar ordem quando apropriado;
- Rejeitar entradas inválidas.

Não executar o texto digitado pelo usuário.

Não usar `eval`, `Function` ou técnicas equivalentes.

---

# Feedback das questões

Após a resposta, informar:

- Se está correta;
- Qual era a resposta esperada;
- Qual conceito foi aplicado;
- Qual foi o provável erro;
- Como resolver;
- Como verificar.

Usar mensagens específicas.

Exemplo inadequado:

```text
Errado.
```

Exemplo adequado:

```text
A resposta não está correta. Ao dividir os dois lados por -2, o sinal da inequação deve ser invertido.
```

## Tentativas

Permitir até três tentativas antes de liberar automaticamente a resolução completa.

O estudante também pode escolher “Mostrar resolução”.

Registrar quantas tentativas foram usadas.

---

# Dicas progressivas

Cada questão deve permitir até três dicas.

Exemplo:

1. Dica conceitual;
2. Dica sobre a próxima operação;
3. Dica quase completa.

Não revelar a resposta já na primeira dica.

Registrar o uso de dicas no progresso.

---

# Resolução passo a passo

As resoluções devem ser apresentadas de forma organizada.

Cada passo deve ter:

- Expressão anterior;
- Operação realizada;
- Expressão resultante;
- Pequena justificativa.

Exemplo:

```text
2x + 6 = 14
2x = 14 - 6        Subtraímos 6 dos dois lados.
2x = 8
x = 8 ÷ 2          Dividimos os dois lados por 2.
x = 4
```

---

# Gerador de questões

Quando houver geração dinâmica, gerar os dados de forma matematicamente controlada.

## Exemplo para equações do primeiro grau

Escolher primeiro a solução:

```text
x = solução inteira
```

Depois escolher coeficientes válidos e calcular o termo restante.

Isso evita questões sem resposta prevista.

Exemplo:

```javascript
const solution = randomInteger(-10, 10);
const a = randomNonZeroInteger(-9, 9);
const b = randomInteger(-20, 20);
const c = a * solution + b;
```

Questão:

```text
ax + b = c
```

Resposta conhecida:

```text
solution
```

## Regras gerais

- Nunca dividir por zero;
- Nunca criar denominador zero;
- Respeitar domínio;
- Evitar resultados excessivamente grandes;
- Gerar respostas inteiras nos níveis básicos;
- Usar frações simples nos níveis intermediários;
- Aumentar a complexidade progressivamente;
- Verificar internamente cada questão criada;
- Impedir questões duplicadas na mesma sessão.

---

# Sistema de progresso

Usar `localStorage`.

Criar um namespace consistente, por exemplo:

```text
plataformaEquacoes.v1
```

Salvar:

- Módulos acessados;
- Módulos concluídos;
- Questões respondidas;
- Acertos;
- Erros;
- Sequência atual;
- Melhor sequência;
- Dicas utilizadas;
- Resoluções abertas;
- Questões marcadas para revisão;
- Questões favoritas;
- Último módulo;
- Última aba;
- Último nível escolhido;
- Tema;
- Tamanho da fonte;
- Preferências de acessibilidade;
- Histórico resumido de sessões;
- Tempo de estudo;
- Data da última atividade.

## Domínio do módulo

Considerar um módulo dominado quando:

- O estudante responder pelo menos 20 questões;
- Obtiver no mínimo 80% de acerto;
- Completar uma sessão de revisão;
- Acertar pelo menos 5 questões intermediárias ou avançadas.

Exibir claramente o que ainda falta.

---

# Caderno de erros

Cada módulo deve ter uma aba “Meus erros”.

Ela deve mostrar:

- Questão;
- Resposta dada;
- Resposta correta;
- Data;
- Número de tentativas;
- Dicas usadas;
- Conteúdo relacionado;
- Resolução;
- Botão “Tentar novamente”;
- Botão “Marcar como revisada”.

Permitir:

- Filtrar por nível;
- Ordenar por data;
- Mostrar apenas não revisadas;
- Limpar erros revisados;
- Exportar erros em JSON.

---

# Favoritos e anotações

Permitir marcar:

- Questões favoritas;
- Exemplos favoritos;
- Trechos teóricos importantes.

Adicionar uma área de anotações pessoais por módulo.

As anotações devem ser salvas no `localStorage`.

Incluir:

- Botão salvar;
- Indicador de salvamento;
- Botão limpar;
- Contagem de caracteres.

Não enviar dados para nenhum serviço externo.

---

# Cronômetro e sessão de estudo

Adicionar um cronômetro opcional.

Funções:

- Iniciar;
- Pausar;
- Retomar;
- Zerar;
- Registrar tempo ao finalizar sessão.

Também incluir um modo de foco com:

- Teoria escondida;
- Apenas uma questão por vez;
- Interface reduzida;
- Sem animações desnecessárias.

---

# Estatísticas

Cada módulo deve mostrar:

- Questões respondidas;
- Acertos;
- Erros;
- Taxa de acerto;
- Média de tentativas;
- Quantidade de dicas usadas;
- Tempo de estudo;
- Desempenho por nível;
- Desempenho por tipo de questão;
- Evolução nas últimas sessões.

Criar gráficos simples usando apenas:

- HTML;
- CSS;
- SVG inline;
- Canvas nativo.

Não usar bibliotecas externas de gráficos.

Os gráficos devem ter alternativa textual acessível.

---

# Pesquisa interna

A página inicial deve possuir uma busca por conteúdos.

A busca deve localizar:

- Módulos;
- Conceitos;
- Fórmulas;
- Exemplos;
- Palavras-chave.

Exibir resultados instantaneamente.

Não precisa pesquisar dentro de outros arquivos em tempo real. Criar no `index.html` um índice local com os dados necessários de todos os módulos.

---

# Navegação

Cada página deve ter:

- Link para o início;
- Menu com todos os módulos;
- Botão anterior;
- Botão próximo;
- Indicador do módulo atual;
- Botão “Continuar estudando”;
- Atalho para prática;
- Atalho para erros;
- Breadcrumbs.

Salvar a última posição de leitura quando possível.

Ao retornar à página, oferecer:

```text
Continuar do último ponto
```

---

# Atalhos de teclado

Implementar atalhos sem interferir na digitação.

Sugestões:

```text
Alt + 1 → Teoria
Alt + 2 → Exemplos
Alt + 3 → Prática
Alt + 4 → Meus erros
Alt + S → Mostrar ou ocultar menu
Alt + T → Alternar tema
Alt + D → Mostrar próxima dica
Alt + Enter → Verificar resposta
Esc → Fechar modal
```

Mostrar uma janela com os atalhos disponíveis.

---

# Configurações

Criar painel de configurações com:

- Tema claro;
- Tema escuro;
- Tema automático;
- Alto contraste;
- Fonte pequena;
- Fonte normal;
- Fonte grande;
- Reduzir animações;
- Sons de feedback;
- Mostrar cronômetro;
- Mostrar progresso;
- Confirmar antes de revelar resposta.

Salvar todas as preferências.

Os sons devem ser gerados opcionalmente com Web Audio API, sem arquivos externos.

Não tocar som automaticamente sem interação do usuário.

---

# Recursos adicionais

Implementar também:

## Modo impressão

Criar CSS com `@media print`.

Na impressão:

- Ocultar menus;
- Ocultar botões;
- Exibir teoria;
- Exibir lista selecionada de exercícios;
- Manter boa legibilidade;
- Evitar fundos escuros.

## Gerar lista para impressão

Permitir escolher:

- Módulo;
- Nível;
- Quantidade;
- Mostrar ou esconder gabarito.

A geração deve ocorrer dentro da própria página.

## Copiar conteúdo

Adicionar botões para copiar:

- Fórmula;
- Exemplo;
- Questão;
- Resolução.

Usar Clipboard API com fallback seguro.

## Compartilhar progresso

Gerar um resumo textual que possa ser copiado.

Exemplo:

```text
Concluí 35% da trilha de equações, com 82% de acerto em 140 questões.
```

---

# Simulados

O arquivo `22-simulados.html` deve oferecer:

## Simulado básico

- 20 questões;
- Conteúdos fundamentais;
- Tempo opcional;
- Resultado detalhado.

## Simulado intermediário

- 30 questões;
- Mistura de conteúdos;
- Dificuldade progressiva.

## Simulado avançado

- 40 questões;
- Conteúdos avançados;
- Problemas de múltiplas etapas.

## Simulado personalizado

Permitir escolher:

- Módulos;
- Níveis;
- Quantidade;
- Tipos de questão;
- Com ou sem tempo;
- Com ou sem dicas.

## Resultado do simulado

Mostrar:

- Nota;
- Percentual;
- Tempo;
- Acertos;
- Erros;
- Questões não respondidas;
- Desempenho por conteúdo;
- Desempenho por nível;
- Sugestões de revisão;
- Lista de erros;
- Botão para refazer apenas os erros;
- Botão para imprimir;
- Botão para salvar resultado.

Durante o simulado, não revelar a resposta após cada questão.

---

# Página de revisão geral

O arquivo `21-revisao-geral.html` deve conter:

- Resumos de todos os módulos;
- Fórmulas principais;
- Erros comuns;
- Checklist de domínio;
- Exercícios mistos;
- Filtro por conteúdo;
- Filtro por dificuldade;
- Revisão de questões erradas;
- Revisão de favoritos;
- Sessão aleatória;
- Plano de revisão sugerido.

Criar recomendações com base no progresso salvo.

Exemplo:

```text
Você teve 58% de acerto em inequações. Revise a inversão do sinal ao multiplicar ou dividir por números negativos.
```

---

# Qualidade do código

O código deve ser:

- Bem organizado;
- Legível;
- Modular, mesmo estando no mesmo HTML;
- Dividido em funções pequenas;
- Comentado onde necessário;
- Sem variáveis globais desnecessárias;
- Sem repetição excessiva;
- Sem erros no console;
- Sem código morto;
- Sem placeholders;
- Sem dados incompletos.

Usar uma estrutura como:

```javascript
(() => {
  'use strict';

  const state = {};
  const storage = {};
  const ui = {};
  const quiz = {};
  const accessibility = {};

  function init() {
    // Inicialização.
  }

  document.addEventListener('DOMContentLoaded', init);
})();
```

---

# Robustez

Tratar:

- `localStorage` indisponível;
- JSON inválido;
- Campos vazios;
- Respostas malformadas;
- Navegador sem Clipboard API;
- Navegador sem Web Audio API;
- Importação de progresso incompatível;
- Sessão sem questões;
- Falta de questões para um filtro;
- Redimensionamento da tela;
- Impressão;
- Preferência de movimento reduzido.

Mostrar mensagens compreensíveis em vez de falhar silenciosamente.

---

# Desempenho

Evitar:

- Milhares de elementos renderizados ao mesmo tempo;
- Recriar toda a página a cada resposta;
- Event listeners duplicados;
- Animações pesadas;
- Grandes intervalos executando continuamente;
- Armazenar dados desnecessários.

Renderizar apenas a questão atual durante sessões.

Usar delegação de eventos quando apropriado.

---

# Conteúdo matemático

Todo resultado matemático deve ser revisado.

Antes de considerar um módulo concluído:

- Conferir exemplos;
- Conferir gabaritos;
- Conferir restrições;
- Conferir sinais;
- Conferir fórmulas;
- Conferir soluções;
- Conferir explicações;
- Conferir se não existem divisões por zero;
- Conferir se soluções inválidas são rejeitadas;
- Conferir se exercícios gerados possuem resposta.

Não inventar regras matemáticas.

---

# Processo de implementação

Execute na seguinte ordem:

## Etapa 1 — Preparação

1. Ler `guia_completo_equacoes_para_codex.md`;
2. Criar uma lista interna de requisitos;
3. Planejar componentes reutilizáveis;
4. Definir chaves do `localStorage`;
5. Definir padrão visual;
6. Definir estrutura dos bancos de questões.

## Etapa 2 — Base visual

1. Criar `index.html`;
2. Criar navegação;
3. Criar temas;
4. Criar acessibilidade;
5. Criar painel de configurações;
6. Criar sistema de progresso.

## Etapa 3 — Primeiro módulo completo

Criar `01-fundamentos-aritmeticos.html` integralmente.

Usar esse módulo como referência de qualidade para os demais.

## Etapa 4 — Demais módulos

Criar todos os módulos em ordem.

Não reduzir a qualidade dos módulos finais.

## Etapa 5 — Revisão e simulados

Criar:

- `21-revisao-geral.html`;
- `22-simulados.html`.

## Etapa 6 — Testes

Testar:

- Links;
- Temas;
- Progresso;
- Importação;
- Exportação;
- Questionários;
- Validação;
- Dicas;
- Resoluções;
- Atalhos;
- Responsividade;
- Impressão;
- Acessibilidade básica;
- Ausência de erros no console.

---

# Regras contra respostas incompletas

Não faça apenas uma explicação do que seria criado.

Crie os arquivos de verdade.

Não encerre após criar um único exemplo.

Não substitua conteúdo por comentários.

Não deixe exercícios sem gabarito.

Não deixe botões sem função.

Não gere uma interface bonita sem conteúdo matemático.

Não gere conteúdo matemático sem interatividade.

Não crie referências a arquivos CSS ou JS externos.

Não use links quebrados.

Não use caminhos absolutos da máquina.

Não dependa de servidor local.

Não remova funcionalidades para economizar código.

Caso o volume seja grande, trabalhe arquivo por arquivo, mas continue até concluir todos.

---

# Critérios de aceitação

O projeto será considerado concluído somente quando:

- Todos os 23 arquivos HTML existirem;
- Todos abrirem diretamente no navegador;
- Todos tiverem CSS e JavaScript embutidos;
- Todos estiverem em português do Brasil;
- Todos tiverem navegação funcional;
- Todos os módulos tiverem teoria;
- Todos os módulos tiverem exemplos;
- Todos os módulos tiverem exercícios;
- Todos os módulos tiverem dicas;
- Todos os módulos tiverem resoluções;
- O progresso funcionar entre páginas;
- O tema funcionar entre páginas;
- A revisão de erros funcionar;
- Os simulados funcionarem;
- A importação e exportação funcionarem;
- O layout for responsivo;
- Não houver erros relevantes no console;
- Não houver placeholders;
- O conteúdo seguir a ordem e os conceitos do guia.

---

# Entrega final

Ao terminar:

1. Liste todos os arquivos criados;
2. Informe quais funcionalidades foram implementadas;
3. Informe como abrir o projeto;
4. Informe quais testes foram realizados;
5. Aponte qualquer limitação real que ainda exista;
6. Não diga que algo foi concluído sem ter sido efetivamente implementado.

Comece agora lendo o arquivo `guia_completo_equacoes_para_codex.md` e criando a plataforma completa.
