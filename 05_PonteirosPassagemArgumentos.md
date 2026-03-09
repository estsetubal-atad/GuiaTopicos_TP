## 5 - Ponteiros e passagem de argumentos

### Exposição

Slides `1 ~ 45`

> Os slides demonstram de uma forma construtiva e simples o conceito de ponteiros e conceitos relacionados.   
> Respondam às questões Quiz dos slides.

### Exercícios

Uma seleção de exercícios de **Ficha | Ponteiros e passagem de argumentos**

### Quiz Moodle

Assíncrono

### TPC - Exploração por LLM

#### Prompt 1 — Debugging com ponteiros

> Estou a aprender ponteiros em C e tenho o seguinte código.
>
> ```c
> #include <stdio.h>
>
> void troca(int *a, int *b) {
>     int *temp;
>     temp = a;
>     a = b;
>     b = temp;
> }
>
> int main() {
>     int x = 5, y = 10;
>     troca(&x, &y);
>     printf("x = %d, y = %d\n", x, y);
>     return 0;
> }
> ```
>
> 1. Explica passo a passo o que acontece na memória quando o programa corre.
> 2. Porque é que os valores de `x` e `y` não são trocados?
> 3. Corrige a função mantendo o uso de ponteiros e explica porque a nova versão funciona.

💡 Alternativamente, coloque o código e execute em <https://pythontutor.com/c.html#> e analise a execução.

🎯 **Objetivo pedagógico:** perceber **passagem por valor vs manipulação do conteúdo apontado**.

---

### Prompt 2 — Visualização de memória

> Estou a estudar ponteiros em C. Analisa o seguinte código e explica detalhadamente o que acontece:
>
> ```c
> #include <stdio.h>
>
> int main() {
>     int a = 10;
>     int *p = &a;
>     int **pp = &p;
>
>     *p = 20;
>     **pp = 30;
>
>     printf("a = %d\n", a);
> }
> ```
>
> 1. Explica o papel de cada variável (`a`, `p`, `pp`).
> 2. Mostra um diagrama simples da memória com os endereços e os valores.
> 3. Explica passo a passo como `a` passa de 10 para 30.

💡 Alternativamente, coloque o código e execute em <https://pythontutor.com/c.html#> e analise a execução.

🎯 **Objetivo pedagógico:** compreender **níveis de indireção (`*` e `**`)**. 


