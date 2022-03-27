# Basic program
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


### `01.01.001` Code mistère 001
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

### `01.01.002` Code mistère 002
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

### `01.01.003` Code mistère 003
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

### `01.01.004` Code mistère 004
`code c`
```c
# include <stdlib.h>
# include <stdio.h>
# define MAX 13

void init(int c, int *mth);
void print(int input, int c, int *mth);

int main() {
    int M[MAX];
    int i;

    init(MAX, M);
    printf("Please, enter a number between 1 and 12 : ");
    scanf("%d", &i);
    
    print(i, MAX, M);
    return EXIT_SUCCESS;

}

void init(int c, int *mth) {
    int k = 0;
    for (k = 1; k < c; k++) {
        if (k == 2) mth[k] = 28;
        else if ((k % 2 == 0 && k <= 7) || (k % 2 == 1 && k > 7))
            mth[k] = 30;
        else
            mth[k] = 31;
    }

}

void print(int input, int c, int *mth) {
    if (input == -1)
        for (int i = 1; i <= c - 1; i ++)
            printf("[%d] == [%d];\n", i, mth[i]);
    else
        printf("FOR %d WE HAVE %d.\n", input, mth[input]);

}

```
1. Imprime sur ta feuille vierge, le résultat qui sera exactement affiché 
à l’écran pour chacune des valeurs suivantes entrées par l'utilisateur :
    - -1
    - 4
    - 9
    - 13
    - 0

2. Dis moi ce que le programme.

<br/>

## Programming
Ici, tu vas pouvoir t'exprimer à travers tes propres lignes de codes. 

> **NOTE** <br/>
> Dans les exercices qui te seront présentés, les `EXEC` représentent les 
> exemples d'exécution souhaités. Dans ces derniers, les lignes 
> commençant par `>_` indiquent les entrées de l'utilisateur (`scanf`) et 
> les autres lignes représentent les affichages du programme (`printf`).

### `01.02.001` Parité d’un entier
Écris un programme qui détermine si un entier saisi est pair ou impair.

`EXEC`
```
>_ 12
12 est un entier pair !

```

### `01.02.002` Équation du premier degré
Écris un programme qui permet de résoudre une équation de degré 1. Je te rappel qu'une équation du premier degré est sous la forme suivante :
    $$ ax + b = 0 $$

Avec $a$ et $b$ deux nombres réels qui représentent les coéfficients
de l'équation. <br/>
La résolution d'une telle équation, revient tout simplement à calculer $x$
avec la formule suivante :
    $$ x = \frac{-b}{a} $$

$x$ est donc la solution de l'équation.

`EXEC`
```
>_ 3x + 4 = 0
La solution de cette equation est : -1.333

```
Assure toi que ton programme affiche la solution avec `3 chiffres` après
la virgule (`.`).


<br/>
<br/>
