# Arrays
- Podemos armazenar difrentes conjuntos de dados deentro de uma unica variável

```
let herois = "Batman", "Homem-Aranha", "Superman"

console.log(herois)
```

**Output:**
> [ 'Batman', 'Homem-Aranha', 'Superman' ]

- Para selecionar um item de uma array devemos lembrar que o Javascript é Zero Based:
- Utiliza-se `[]` após o nome da variável

```
console.log(herois[0])
console.log(herois[3 - 1])
```
**Output:**
>  Batman
>
>  Superman

## Sobrescrever valores de uma array
- Para atribuir umn novo valor a um item de uma array, devemos utilizar:

``` 
herois[1] = "Mulher Gato"
conosle.log(herois)
```
**Output:**
> [ 'Batman', 'Mulher Gato', 'Superman' ]

## Difrentes tipos de dados em uma array
- Podemos misturar tipos de dados, como numbers e strings dentro de uma unica array:

```
let idadeAposentadoria = ["Homem", "Mulher", 65, 62]
```
**Output:**
> [ 'Homem', 'Mulher', 65, 62 ]

## Métodos de arrays
### Length
- Retorna a quantidade de itens dentro de uma array
```
console.log(herois.length)
```
**Output:**
> 3

### Join()
- Retorna uma string com todos os itens de uma array concatenados e separados

```
console.log(herois.join('|'))
console.log(herois.join('-'))
```
**Output:**
> Batman | Homem-Aranha | Superman
>
> Batman - Homem-Aranha - Superman

### indexOf()
- Retorna a posição de um item expecificado, sendo numero ou string, dentro de uma array
- Apenas retorna a primeira ocorrência

```
const idade = [31, 42, 15, 18, 42]
console.log(idade.indexOf(42))
```
**Output:**
> 1
- Caso um valor expecificado não exista dentro da array, será exibido no console o valor `-1`

### concat()
- Concatena 2 arrays
- **Não Modifica** a array original

```
const maisHerois = herois.concat(["Doutor Estranho", "Aquaman"])
```
**Output:**
> [ 'Batman', 'Homem-Aranha', 'Superman', 'Doutor Estranho', 'Aquaman' ]

### Push()
- Adiciona itens à array
- **Modifica** a array original (mutação de valores)
- Retorna a quantiadde de itens dentro da array

```
console.log(herois.push("Hulk", "Aquaman"))
console.log(herois)
```
**Output:**
> 5

> [ 'Batman', 'Homem-Aranha', 'Superman', 'hulk', 'Aquaman' ]

### Pop()
- **Remove** o útimo item dentro da array
- Retorna o item removido

```
console.log(herois.pop())
console.log(herois)
```
**Output:**
> Aquaman

> [ 'Batman', 'Homem-Aranha', 'Superman', 'hulk' ]