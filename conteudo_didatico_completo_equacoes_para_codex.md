# Material didático completo de Álgebra, Equações, Inequações, Funções e Sistemas

## Documento-base para geração de páginas HTML pelo Codex

Este arquivo contém o conteúdo pedagógico que deve alimentar a plataforma de estudos. Ele não é apenas um índice: cada tópico precisa ser transformado pelo Codex em teoria, exemplos resolvidos, atividades, dicas progressivas, feedbacks e resoluções passo a passo.

O público pode incluir crianças mais velhas, adolescentes e adultos. Por isso, cada assunto deve começar com uma explicação intuitiva e depois apresentar a forma matemática.

---

# 1. Diretrizes pedagógicas gerais

## 1.1 Linguagem

A linguagem deve ser clara, direta, respeitosa e sem infantilização. Nenhum símbolo ou termo técnico deve ser usado pela primeira vez sem explicação.

Exemplo adequado:

> **Incógnita** é o valor desconhecido que queremos descobrir. Geralmente, ela é representada por uma letra, como \(x\).

Evitar:

> “Passa para o outro lado e troca o sinal.”

Preferir:

> “Subtraímos \(5\) dos dois lados da igualdade. Assim, preservamos o equilíbrio da equação.”

A expressão informal “passar para o outro lado” pode aparecer como atalho, mas a operação real deve ser explicada.

## 1.2 Estrutura de cada tópico

Cada tópico deve seguir esta ordem:

1. Ideia intuitiva;
2. Definição;
3. Vocabulário;
4. Regra ou fórmula;
5. Exemplo básico;
6. Exemplo intermediário;
7. Exemplo avançado;
8. Verificação;
9. Erros comuns;
10. Exercícios;
11. Resumo.

## 1.3 Formatação matemática

Usar LaTeX.

Em linha:

```text
A forma geral é \(ax+b=0\).
```

Em bloco:

```text
\[
ax+b=0
\]
```

Frações:

\[
\frac{a}{b}
\]

Raízes:

\[
\sqrt{x}
\]

Sistemas:

\[
\begin{cases}
x+y=10\\
x-y=2
\end{cases}
\]

Intervalos:

\[
x\in[2,5)
\]

Não usar formas improvisadas em explicações principais quando houver uma notação matemática melhor.

## 1.4 Progressão de dificuldade

### Básico

- Números inteiros pequenos;
- Uma ideia por exercício;
- Poucos passos;
- Respostas inteiras.

### Intermediário

- Números negativos;
- Frações simples;
- Parênteses;
- Mais de uma etapa.

### Avançado

- Frações algébricas;
- Restrições;
- Vários métodos;
- Problemas contextualizados;
- Casos especiais.

---

# 2. Módulo 0 — Fundamentos aritméticos

## 2.1 Objetivo

Revisar operações essenciais para que erros de cálculo não prejudiquem o aprendizado de álgebra.

## 2.2 Conjuntos numéricos

### Números naturais

Usados para contar:

\[
\mathbb{N}=\{0,1,2,3,\ldots\}
\]

### Números inteiros

Incluem negativos, zero e positivos:

\[
\mathbb{Z}=\{\ldots,-3,-2,-1,0,1,2,3,\ldots\}
\]

### Números racionais

Podem ser escritos como:

\[
\frac{a}{b}
\]

com \(a,b\in\mathbb{Z}\) e \(b\neq0\).

Exemplos:

\[
\frac{1}{2},\quad -3,\quad 0{,}75,\quad 0{,}333\ldots
\]

### Números irracionais

Não podem ser escritos como fração de inteiros:

\[
\sqrt{2},\quad \pi
\]

### Números reais

Reúnem racionais e irracionais:

\[
\mathbb{R}
\]

## 2.3 Reta numérica

Na reta numérica:

- Números maiores ficam à direita;
- Números menores ficam à esquerda;
- O zero separa positivos e negativos.

\[
-5<-2<0<3<8
\]

Logo:

\[
-2>-5
\]

## 2.4 Valor absoluto

Representa a distância até o zero:

\[
|5|=5
\]

\[
|-5|=5
\]

Formalmente:

\[
|x|=
\begin{cases}
x, & x\geq0\\
-x, & x<0
\end{cases}
\]

## 2.5 Adição de inteiros

### Sinais iguais

Somar os valores e manter o sinal:

\[
5+3=8
\]

\[
-5+(-3)=-8
\]

### Sinais diferentes

Subtrair os valores absolutos e usar o sinal do maior em valor absoluto:

\[
8+(-3)=5
\]

\[
-8+3=-5
\]

## 2.6 Subtração de inteiros

Subtrair é somar o oposto:

\[
a-b=a+(-b)
\]

Exemplos:

\[
7-3=4
\]

\[
7-(-3)=7+3=10
\]

\[
-4-6=-10
\]

## 2.7 Multiplicação e divisão com sinais

\[
(+)\cdot(+)=+
\]

\[
(+)\cdot(-)=-
\]

\[
(-)\cdot(+) = -
\]

\[
(-)\cdot(-)=+
\]

Exemplos:

\[
(-4)\cdot3=-12
\]

\[
(-4)\cdot(-3)=12
\]

\[
\frac{-20}{5}=-4
\]

\[
\frac{-20}{-5}=4
\]

## 2.8 Ordem das operações

1. Parênteses;
2. Potências e raízes;
3. Multiplicações e divisões;
4. Adições e subtrações.

Exemplo:

\[
3+2\cdot5
\]

\[
3+10=13
\]

Com parênteses:

\[
(3+2)\cdot5=25
\]

## 2.9 Frações

Na fração:

\[
\frac{3}{5}
\]

- \(3\) é o numerador;
- \(5\) é o denominador.

O denominador nunca pode ser zero.

### Frações equivalentes

\[
\frac{1}{2}=\frac{2}{4}=\frac{3}{6}
\]

### Simplificação

\[
\frac{12}{18}=\frac{2}{3}
\]

### Soma com denominadores iguais

\[
\frac{2}{7}+\frac{3}{7}=\frac{5}{7}
\]

### Soma com denominadores diferentes

\[
\frac{1}{2}+\frac{1}{3}
=
\frac{3}{6}+\frac{2}{6}
=
\frac{5}{6}
\]

### Multiplicação

\[
\frac{2}{3}\cdot\frac{5}{4}
=
\frac{10}{12}
=
\frac{5}{6}
\]

### Divisão

\[
\frac{2}{3}\div\frac{5}{4}
=
\frac{2}{3}\cdot\frac{4}{5}
=
\frac{8}{15}
\]

## 2.10 Decimais e porcentagens

\[
0{,}5=\frac{1}{2}
\]

\[
25\%=\frac{25}{100}=0{,}25
\]

Para calcular \(20\%\) de \(150\):

\[
\frac{20}{100}\cdot150=30
\]

## 2.11 Potenciação

Em:

\[
a^n
\]

\(a\) é a base e \(n\) é o expoente.

\[
2^4=16
\]

Para \(a\neq0\):

\[
a^0=1
\]

\[
a^{-n}=\frac{1}{a^n}
\]

Cuidado:

\[
(-3)^2=9
\]

mas:

\[
-3^2=-9
\]

## 2.12 Radiciação

\[
\sqrt{25}=5
\]

A raiz quadrada principal é não negativa.

Ao resolver:

\[
x^2=25
\]

temos:

\[
x=\pm5
\]

## 2.13 Exercícios

1. \(7+(-12)\)
2. \(-5-(-8)\)
3. \((-6)(-4)\)
4. \(18\div(-3)\)
5. \(3+4\cdot2\)
6. \((3+4)\cdot2\)
7. Simplifique \(\frac{18}{24}\).
8. \(\frac{2}{3}+\frac{1}{6}\)
9. \(15\%\) de \(200\)
10. \((-2)^4\)

### Respostas

1. \(-5\)
2. \(3\)
3. \(24\)
4. \(-6\)
5. \(11\)
6. \(14\)
7. \(\frac{3}{4}\)
8. \(\frac{5}{6}\)
9. \(30\)
10. \(16\)

---

# 3. Módulo 1 — Expressões algébricas

## 3.1 O que é álgebra

Álgebra usa letras e símbolos para representar números e relações.

\[
3+5=8
\]

é uma conta específica. Já:

\[
x+5
\]

representa uma expressão cujo valor depende de \(x\).

## 3.2 Variável e incógnita

### Variável

Pode assumir diferentes valores.

\[
y=2x+1
\]

### Incógnita

É um valor desconhecido:

\[
x+5=12
\]

## 3.3 Expressão algébrica

Combina números, letras e operações:

\[
3x+5
\]

\[
2a-4b
\]

\[
x^2+2x+1
\]

## 3.4 Termos

Na expressão:

\[
4x^2-3x+7
\]

os termos são:

\[
4x^2,\quad -3x,\quad 7
\]

O sinal pertence ao termo.

## 3.5 Coeficiente e parte literal

Em:

\[
-5x^2y
\]

- Coeficiente: \(-5\);
- Parte literal: \(x^2y\).

Em \(x\), o coeficiente é \(1\).

Em \(-x\), o coeficiente é \(-1\).

## 3.6 Grau

O grau de um termo é a soma dos expoentes:

\[
4x^2y^3
\]

tem grau:

\[
2+3=5
\]

O grau de um polinômio é o maior grau entre seus termos.

## 3.7 Classificação

- Monômio: um termo;
- Binômio: dois termos;
- Trinômio: três termos;
- Polinômio: um ou mais termos.

## 3.8 Valor numérico

Para:

\[
2x+3
\]

com \(x=4\):

\[
2(4)+3=11
\]

Com número negativo, usar parênteses:

\[
x^2
\]

para \(x=-3\):

\[
(-3)^2=9
\]

## 3.9 Tradução de frases

- Um número: \(x\);
- Dobro: \(2x\);
- Triplo: \(3x\);
- Metade: \(\frac{x}{2}\);
- Sucessor: \(x+1\);
- Antecessor: \(x-1\);
- Quadrado: \(x^2\);
- Dois consecutivos: \(x\) e \(x+1\).

“O quadrado da soma de \(x\) e \(3\)”:

\[
(x+3)^2
\]

“A soma do quadrado de \(x\) com \(3\)”:

\[
x^2+3
\]

## 3.10 Exercícios

1. Identifique os termos de \(5x^2-2x+8\).
2. Qual é o coeficiente de \(-7y\)?
3. Qual é a parte literal de \(4a^2b\)?
4. Qual é o grau de \(3x^2y^4\)?
5. Calcule \(2x+5\) para \(x=3\).
6. Escreva “o triplo de um número diminuído em \(4\)”.
7. Escreva “o quadrado da diferença entre \(x\) e \(2\)”.

### Respostas

1. \(5x^2\), \(-2x\) e \(8\)
2. \(-7\)
3. \(a^2b\)
4. \(6\)
5. \(11\)
6. \(3x-4\)
7. \((x-2)^2\)

---

# 4. Módulo 2 — Redução de termos semelhantes

## 4.1 Conceito

Termos semelhantes possuem exatamente a mesma parte literal.

Exemplos:

\[
3x\quad\text{e}\quad8x
\]

\[
2x^2\quad\text{e}\quad-5x^2
\]

Não são semelhantes:

\[
3x\quad\text{e}\quad3x^2
\]

\[
2x\quad\text{e}\quad2y
\]

## 4.2 Regra

\[
ax+bx=(a+b)x
\]

A parte literal permanece e os coeficientes são combinados.

## 4.3 Exemplos

\[
4x+3x=7x
\]

\[
9y-2y=7y
\]

\[
5a-8a=-3a
\]

Com constantes:

\[
4x+3-2x+5
\]

\[
4x-2x+3+5
\]

\[
2x+8
\]

Com potências:

\[
3x^2+5x-2x^2+7x
\]

\[
x^2+12x
\]

Com várias letras:

\[
2ab+5a-3ab+4a
\]

\[
-ab+9a
\]

## 4.4 Coeficiente implícito

\[
x=1x
\]

\[
-x=-1x
\]

Logo:

\[
x+4x=5x
\]

\[
-x+3x=2x
\]

## 4.5 Erros comuns

Errado:

\[
3x+4y=7xy
\]

Correto:

\[
3x+4y
\]

Errado:

\[
2x+3x^2=5x^3
\]

Correto:

\[
2x+3x^2
\]

## 4.6 Procedimento

1. Identifique os termos;
2. Observe os sinais;
3. Agrupe partes literais iguais;
4. Some os coeficientes;
5. Preserve a parte literal;
6. Verifique se ainda há termos semelhantes.

## 4.7 Exercícios

1. \(3x+8x\)
2. \(9a-12a\)
3. \(4y+7-2y+5\)
4. \(3x^2+2x-5x^2+9x\)
5. \(2ab-7ab+3a\)
6. \(x-x+5\)
7. \(-x-4x+2\)

### Respostas

1. \(11x\)
2. \(-3a\)
3. \(2y+12\)
4. \(-2x^2+11x\)
5. \(-5ab+3a\)
6. \(5\)
7. \(-5x+2\)

---

# 5. Módulo 3 — Propriedade distributiva

## 5.1 Ideia intuitiva

\[
3(x+2)
\]

equivale a três grupos de \(x+2\):

\[
(x+2)+(x+2)+(x+2)
\]

Logo:

\[
3(x+2)=3x+6
\]

## 5.2 Regra

\[
a(b+c)=ab+ac
\]

\[
a(b-c)=ab-ac
\]

## 5.3 Exemplos básicos

\[
4(x+3)=4x+12
\]

\[
5(2x-1)=10x-5
\]

\[
-3(x+4)=-3x-12
\]

\[
-2(x-5)=-2x+10
\]

## 5.4 Distributiva e termos semelhantes

\[
3(x+2)+2x
\]

\[
3x+6+2x
\]

\[
5x+6
\]

Exemplo:

\[
2(3x-4)-5(x+1)
\]

\[
6x-8-5x-5
\]

\[
x-13
\]

## 5.5 Menos antes dos parênteses

\[
-(x+3)=-x-3
\]

\[
-(x-4)=-x+4
\]

## 5.6 Distributiva dupla

\[
(a+b)(c+d)=ac+ad+bc+bd
\]

Exemplo:

\[
(x+2)(x+3)
\]

\[
x^2+3x+2x+6
\]

\[
x^2+5x+6
\]

## 5.7 Erros comuns

Errado:

\[
3(x+2)=3x+2
\]

Correto:

\[
3x+6
\]

Errado:

\[
-2(x-3)=-2x-6
\]

Correto:

\[
-2x+6
\]

## 5.8 Exercícios

1. \(3(x+5)\)
2. \(-4(x-2)\)
3. \(2(3x+1)+x\)
4. \(5(x-2)-3(x+4)\)
5. \((x+1)(x+4)\)
6. \(-(2x-7)\)

### Respostas

1. \(3x+15\)
2. \(-4x+8\)
3. \(7x+2\)
4. \(2x-22\)
5. \(x^2+5x+4\)
6. \(-2x+7\)

---

# 6. Módulo 4 — Equações do primeiro grau

## 6.1 Definição

Uma equação é uma igualdade com uma incógnita:

\[
2x+3=11
\]

Resolver significa encontrar os valores que tornam a igualdade verdadeira.

## 6.2 Princípio da balança

Se:

\[
a=b
\]

então podemos realizar a mesma operação nos dois lados:

\[
a+c=b+c
\]

\[
a-c=b-c
\]

\[
ac=bc
\]

e, para \(c\neq0\):

\[
\frac{a}{c}=\frac{b}{c}
\]

## 6.3 Forma geral

\[
ax+b=0
\]

com:

\[
a\neq0
\]

## 6.4 Equações simples

\[
x+5=12
\]

Subtraindo \(5\) dos dois lados:

\[
x=7
\]

\[
3x=18
\]

Dividindo por \(3\):

\[
x=6
\]

\[
\frac{x}{5}=7
\]

Multiplicando por \(5\):

\[
x=35
\]

## 6.5 Duas etapas

\[
2x+4=14
\]

\[
2x=10
\]

\[
x=5
\]

Verificação:

\[
2(5)+4=14
\]

## 6.6 Incógnita nos dois lados

\[
5x+2=3x+10
\]

\[
2x+2=10
\]

\[
2x=8
\]

\[
x=4
\]

## 6.7 Com parênteses

\[
3(x+2)=15
\]

\[
3x+6=15
\]

\[
3x=9
\]

\[
x=3
\]

## 6.8 Com termos semelhantes

\[
4x+3-2x=11
\]

\[
2x+3=11
\]

\[
2x=8
\]

\[
x=4
\]

## 6.9 Com frações

\[
\frac{x}{3}+2=6
\]

\[
\frac{x}{3}=4
\]

\[
x=12
\]

Com vários denominadores:

\[
\frac{x}{2}+\frac{x}{3}=10
\]

Multiplicando tudo por \(6\):

\[
3x+2x=60
\]

\[
5x=60
\]

\[
x=12
\]

## 6.10 Com decimais

\[
0{,}5x+1=4
\]

\[
0{,}5x=3
\]

\[
x=6
\]

## 6.11 Tipos de solução

### Uma solução

\[
2x+3=11
\]

\[
x=4
\]

### Infinitas soluções

\[
2(x+3)=2x+6
\]

\[
2x+6=2x+6
\]

\[
S=\mathbb{R}
\]

### Nenhuma solução

\[
2x+3=2x+8
\]

\[
3=8
\]

\[
S=\varnothing
\]

## 6.12 Método geral

1. Elimine parênteses;
2. Elimine denominadores;
3. Reduza termos semelhantes;
4. Reúna os termos com incógnita;
5. Reúna os termos constantes;
6. Isole a incógnita;
7. Verifique;
8. Escreva o conjunto solução.

## 6.13 Erros comuns

- Trocar sinais sem explicar a operação;
- Dividir apenas parte de uma expressão;
- Perder sinais negativos;
- Não verificar;
- Esquecer casos de infinitas soluções e sem solução.

## 6.14 Exercícios

1. \(x+8=21\)
2. \(4x=28\)
3. \(3x-5=16\)
4. \(7x+2=5x+18\)
5. \(2(x+4)=18\)
6. \(3(x-2)+x=12\)
7. \(\frac{x}{4}+3=8\)
8. \(\frac{x}{2}+\frac{x}{5}=14\)
9. \(2x+7=2x+7\)
10. \(5x+1=5x-3\)

### Respostas

1. \(x=13\)
2. \(x=7\)
3. \(x=7\)
4. \(x=8\)
5. \(x=5\)
6. \(x=\frac{9}{2}\)
7. \(x=20\)
8. \(x=20\)
9. Infinitas soluções
10. Sem solução

---
