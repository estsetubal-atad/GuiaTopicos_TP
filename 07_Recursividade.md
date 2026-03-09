## 7 - Recursividade

### Exposição

Slides `1 ~ 35`

> Os slides demonstram de uma forma construtiva e simples o conceito de recursividade.
> Respondam às questões Quiz dos slides.  
> Façam os exercícios propostos em aula.

### Quiz Moodle

Assíncrono

### TPC 

Elaborar exercícios para TPC (slides).

Complementar com **`Ficha | Recursividade`** (Moodle)

### TPC - Exploração por LLM

Por forma a tentar combinar os conceitos de recursividade e ponteiros, tente chegar a uma solução para a seguinte função recursiva (não peça a solução, peça para guiá-lo para uma solução, i.e.. com **boas práticas LLM**).

*Variante* recursiva de `isPalindromo` que utiliza dois ponteiros: um para o caractere inicial, outro para o final:

```cpp
int isPalindromo(char *start, char *end) {
    // TODO
}
```

:bulb: Esta versão é interessante pois terá de utilizar **aritmética de ponteiros** e **derreferenciação**.

Uso:

```cpp
char str[] = "radar"; // teste com outras palavras

int res = isPalindromo(str, str + strlen(str) - 1);

printf("isPalindromo? = %d\n", res);
```


