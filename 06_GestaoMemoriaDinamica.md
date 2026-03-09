## 6 - Ponteiros e gestão de memória dinâmica (heap)

### Exposição

Slides `1 ~ 36`

> Os slides demonstram de uma forma construtiva e simples o conceito de ponteiros e gestão de memória dinâmica.  
> Respondam às questões Quiz dos slides.  
> Façam os exercícios propostos em aula.


### Quiz Moodle

Assíncrono

### TPC - Ficha

Exercícios de **Ficha | Gestão de memória dinâmica**

### TPC - Exploração por LLM

Exploração de uma curiosidade da linguagem C; tente encontrar a resposta...

Considere o seguinte código:

```cpp
#include <stdio.h>
#include <stdlib.h>

typedef struct {
    char a;
    int b;
    char c;    
} SomeStruct;

int main() {
    
    SomeStruct s;
    printf("%ld\n", sizeof(s));

    return 0;
}
```

- Provavelmente esperaria que o *output* fosse `6`, i.e., a soma dos tamanhos das variáveis (`1 + 4 + 1)` - o que faz todo o sentido! 
- Mas se correr o programa irá ver que o *output* é `12`!
- E se modificar a estrutura para:

    ```cpp
    typedef struct {
        char a;
        char b;
        int c;    
    } SomeStruct;
    ```

    Irá verificar que o *output* é `8`!