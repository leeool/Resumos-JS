# Números em Javascript
## Ordem das Operações
1. Parenteses
2. Expoentes e raizes
3. Multiplicação e divisão
4. Soma e subtração

## Incremento e decremento
- Podemos incrementar ou decrementar valores de uma variável
- Usamos `let` pois a variável alterará seu valor
```
let numeroIncremento = 10
numeroIncremento++
let numeroDecremento = 10
numeroDecremento--


console.log(numeroDecremento)
console.log(numeroIncremento)
```

**Output:**
>9

> 11

## Operadores de assignments
-  Faz uma variável receber um valor específicado

```
let postLikes = 10

postLikes += 10
console.log(postLikes)

postLikes = 10
postLikes -= 10
console.log(postLikes)

postLikes = 10
postLikes /= 2
console.log(postLikes)

postLikes = 10
postLikes *= 3
console.log(postLikes)

```
**Output:**
>20

> 0

> 5

> 30

## Concatenação de números com strings
- O javascript converte números em strings após a concatenação

```
const likeMessage = "O post tem " + postLikes + " likes"
console.log(likeMessage)
```
**Output:**
>O post tem 30 likes