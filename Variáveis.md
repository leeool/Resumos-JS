## Tipos de variáveis em Javascript

- let
- const
- var 

- (**let** e **const** são as variáveis mais usadas atualmente)

### let
A keyword `let` pode ser usada para criar uma variável de nome opcional, logo em seguida, usamos o `=` junto com um valor para armazenar uma informação dentro da variável criada. Ex.:
`let idade = 17;`

É importante lembrar que o código é lido de cima para baixo, ou seja, podemos alterar o valor da variável ao definirmos um novo valor durante o código.
`idade = 18;`

### const
Ao contrario de `let`, a keyword `const` não pode ser alterada ao decorrer do código, como podemos supor (const = constante) sendo uma variável de valor imutável. Se caso mudarmos o valor, resultará em erro no código, já que não podemos alterar valores de uma const. 

```
const idade = 1;
idade = 1;
erro.
```

### var
Antigamente, a keyword `var` era a única forma de criar uma variável dentro do Javascript, tendo uma funcionalidade parecida com `let`, já que também podemos alterar seu valor.

## Boas-Práticas

### Convenção Camel Case
Convenção usada em Javascript, na qual foi determinado que o modo correto de nomear variáveis siga um determinado "template" para que seu código seja mais legível.
- Camel Case significa "Caixa de Camelo"

Ex.:
```
let anoAtual = 2022;
let mesAniversárioPai = "maio";
```
Pode-se notar que a frase que denomina a variável é iniciada por uma letra minúscula e as seguintes palavras são iniciadas por letras maiúsculas. 

### Variáveis com nomes claros
É importante nomear variáveis com frases que sejam fáceis de identificar, facilitando o entendimento do seu código para outros desenvolvedores no futuro, sendo uma importante prática para quem irá trabalhar em equipes. 

