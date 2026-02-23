## 3 - Algoritmos: formalização, complexidades e análise

### Exposição

Slides `1 ~ 21`.

### Exploração por LLM

> Na aula anterior já vimos alguns tipos primitivos, e.g., `int` e `float` e derivados, e.g., *arrays* de inteiros.

**Prompt 1:**

```console
Explica o conceito de complexidade algorítmica como se eu fosse um estudante do primeiro ano de engenharia. Usa exemplos do dia a dia e evita formalismo matemático. Se for necessário incluir código, usa a linguagem C.
```

**Prompt 2:**

```console
O que é a notação Big-O? 
```

> Se não incluir na resposta, pergunte sobre "classes de complexidades algorítmicas".

**Prompt 3:**

```console
Mostra-me dois algoritmos que resolvam o mesmo problema - um problema simples sem arrays, mas com complexidades algorítmicas diferentes.
```

**Prompt 4:**

```console
Agora um problema que envolva arrays.
```

**Prompt 5:**

```console
Que passos deverei seguir para analisar a complexidade de um algoritmo? 
```

**Prompt 6:**

```console
Cria-me um pequeno problema para eu estimar a complexidade algorítmica na notação Big-O. 
```

### Exposição

Slides `22 ~ 28`.

### Quiz em Aula

Responder às questões dos Quiz.

### Análise de Complexidade Algorítmica

Considere as seguintes matrizes:

#### Matriz A (m × n)

$$
A =
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix}
$$

#### Matriz B (n × n)

$$
B =
\begin{bmatrix}
b_{11} & b_{12} & \dots & b_{1n} \\
b_{21} & b_{22} & \dots & b_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
b_{n1} & b_{n2} & \dots & b_{nn}
\end{bmatrix}
$$

---

#### Questões

1. Qual é a complexidade temporal para calcular a soma de todos os elementos da matriz **A**?

2. Qual é a complexidade temporal para calcular a soma de todos os elementos da matriz **B**?

3. Qual é a complexidade temporal para calcular apenas a soma da diagonal principal da matriz **B**?

4. Compare os resultados obtidos e explique:
   - Porque a soma da matriz completa difere da soma da diagonal?
   - Como a dimensão da entrada influencia a notação Big-O?

**Sugestão**:

Considere que:
- A matriz A tem dimensão \( m \times n \)
- A matriz B tem dimensão \( n \times n \)
- Cada acesso a um elemento da matriz tem custo constante \( O(1) \)

### Ficha

Fazer a ficha na 2ª aula do tópico.

### Quiz Moodle

Assíncrono.
