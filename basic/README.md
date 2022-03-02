# Basic programme
Ici, tu vas affronter les codes les plus simple et basique pour commencer
la programmation.

<br/>

## Code hacking
Dans cette section, tu vas tenter de hacker des codes sources afin de
t'imprégner du fonctionnement d'un programme informatique. Ce défit te
permettra de maîtriser l'agorithmique de façon basique.

> **WARNING**<br/>
> Il est formellement interdit d'utiliser un ordinateur pour compiler
> les codes sources qui se trouve dans cette section `Code hacking`.


### 01.001. Code mistère 001
`code c`
```c
# include <stdlib.h>
# include <stdio.h>

int main() {
    int u0 = 0;
    int u1 = 1;
    int un;

    for (int i = 0; i < 10; i++) {
        un = u0 + u1;
        u0 = u1;
        u1 = un;
    }

    printf("U0 = %d\nU1 = %d\n", u0, u1);
    return EXIT_SUCCESS;

}

```
Imprime sur ta feuille vierge, le résultat qui sera exactement affiché
à l'écran lorsqu'on exécutera le code source ci-dessus.

### 01.002 Code mistère 002
`code c`
```c
# include <stdlib.h>
# include <stdio.h>

int main() {
    int x = 10;

    // printf("I'm there to print to your terminal !\n");
    // x = 200;
    for (; x < 10; x++)
        printf("x == %d\n", x);

    return EXIT_SUCCESS;

}

```
Imprime sur ta feuille vierge, le résultat qui sera exactement affiché
à l'écran lorsqu'on exécutera le code source ci-dessus.

### 01.003 Code mistère 003
`code c`
```c
# include <stdlib.h>
# include <stdio.h>

void exg(int a, int b) {
    int c = a;
    a = b;
    b = c;

}

int main() {
    int a = 10;
    int b = 20;

    exg(a, b);
    printf("a = %d, b = %d", a, b);
    return EXIT_SUCCESS;

}

```
1. Imprime sur ta feuille vierge, le résultat qui sera exactement affiché
à l'écran lorsqu'on exécutera le code source ci-dessus.
2. Explique moi ce qui s'est passé.

<br/>
<br/>
