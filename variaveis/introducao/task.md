
## O que é uma variável?

Uma variável é um armazenamento para um valor, que pode ser uma string, um número ou qualquer outra coisa. Cada variável tem um **nome** (ou um **identificador** ) para distingui-la de outras variáveis. Você pode acessar um valor pelo nome da variável.

As variáveis são um dos elementos mais usados em programas; portanto, é importante entender como usá-los.

## Declarando variáveis

Antes de começar a usar uma variável, você deve declará-la. Para declarar uma variável, o Kotlin fornece duas palavras-chave:

-   `val` (para _valor_ ) declara uma **variável imutável** (apenas um **valor nomeado** ou uma **constante** ), que não pode ser alterada após ter sido inicializada;
-   `var` (para _variavel_ ) declara uma **variável mutável** , que pode ser alterada (quantas vezes forem necessárias).

Ambas as palavras-chave `val` e `var` fornecem uma variável!

Ao declarar uma variável, você deve adicionar seu nome após uma dessas duas palavras-chave. Cuidado: o nome de uma variável não pode começar com um dígito. Normalmente, começa com uma letra. Você deve escolher nomes significativos e legíveis para variáveis para tornar seu código fácil de entender.

Para atribuir um determinado valor a uma variável, devemos usar o operador de atribuição `=`.

Vamos declarar uma variável imutável chamada `linguagem` e inicializá-la com a string `"Kotlin"`.

```kotlin
val linguagem = "Kotlin"
```

Agora podemos acessar essa string pelo nome da variável. Vamos imprimir!

```kotlin
println(language) // impressão "Kotlin" sem aspas
```

Esta variável não pode ser modificada após ter sido inicializada porque foi declarada como `val`.

Os nomes diferenciam maiúsculas de minúsculas: `linguagem` não é o mesmo que `Linguagem`.

Agora, vamos declarar uma variável mutável nomeada `diaDaSemana` e imprimir seu valor antes e depois de alterá-la.

```kotlin
var diaDaSemana = "Segunda-Feira" 
println(diaDaSemana) // imprimir Segunda-Feira 
diaDaSemana = "Terça-Feira" 
println(diaDaSemana) // imprime Terça-Feira
```

No exemplo acima, declaramos uma variável nomeada `diaDaSemana` e a inicializamos com o valor `"Segunda-Feira"`. Em seguida, acessamos o valor pelo nome da variável e o imprimimos. Depois disso, alteramos o valor da variável `"Terça-Feira"` e imprimimos esse novo valor.

Você não precisa declarar uma variável novamente para alterar seu valor. Basta atribuir um novo valor a ele usando o operador `=` (igual).

Também é possível declarar e inicializar uma variável com o valor de outra variável:

```kotlin
val custo = 3
val custoDoCafe = custo 
println(custoDoCafe) // imprime 3
```

## Armazenando diferentes tipos de valores

Já mencionamos que as variáveis podem armazenar diferentes tipos de valores: strings, números, caracteres e outros tipos de dados.

Vamos declarar três variáveis imutáveis para armazenar um número, uma string e um caractere e então imprimir seus valores.

```kotlin
val dez = 10 
val saudacao = "Olá" 
val primeiraLetra = 'A' 

println(dez) // imprimie 10 
println(saudacao) // imprime Olá
println(primeiraLetra) // imprime A
```

`var` No entanto, há uma restrição para variáveis mutáveis (as declaradas com a palavra-chave ). Ao reatribuir seus valores, você só pode usar novos valores do mesmo tipo que o inicial. Portanto, o trecho de código abaixo não está correto:

```kotlin
var numero = 10 
number = 11 // ok
number = "dozse" // um erro aqui!
```

Por favor, lembre-se desta restrição!

## Conclusão

Agora você sabe, existem duas palavras-chave que são usadas para declarar variáveis. Na verdade, em muitos casos, é melhor usar variáveis imutáveis (aquelas declaradas com a palavra-chave `val`). Antes de usar `var`, você deve certificar-se de que `val`não é adequado nesse caso. Se realmente não for, use `var`. Embora, tenha em mente que quanto mais variáveis mutáveis em seu código, mais difícil é ler. Lembre-se, variáveis imutáveis ajudam a escrever código mais legível. Então, por favor, use `val`sempre que possível! Você pode substituí-lo facilmente `var`quando for absolutamente necessário.