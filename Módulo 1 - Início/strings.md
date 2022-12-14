# Strings

- Strings são encadeamento de caracteres que devem ser sempre explicitas dentro de aspas (duplas ou simples)
- **Qualquer** caractere dentro de aspas é uma string, tanto letras quanto numeros
- Podemos armazenar strings dentro de variaveis
```
const primeiroNome = "Leonardo"
const ultimoNome = "Gonsalez"
console.log(primeiroNome)
```

# Concatenação de strings
- "Concatenar" é o nome técnico para "juntar"
- Podemos juntar duas ou mais strings no Javascript utilizando `+` entre elas

Ex.:

```
const nomeCompleto = primeiroNome + " " + ultimoNome
console.log(nomeCompleto)
```

# Acessando caracteres
- Em Javascript podemos "selecionar" caracteres de uma variavel string utilizando `[]` e colocando a posição do caractere opcional.

Ex.:
```
console.log(nomeCompleto[0])
console.log(nomeCompleto[5])
```
**Output:**
> L

> r

- Devemos lembrar que Javascript é uma linguagem "Zero Based", ou seja, a contagem sempre começa a partir do zero.

# Propriedade Length
- Retorna a quantidade de caracteres de uma string 
- Deve seguir o template: "[variável].length"
```
console.log(nomeCompleto.length)
```
**Output:**
> 17

- Conta todos os espaços de uma string, inclusive os espaços vazios

# Métodos de string
- Em essencia são a mesma coisa que funções
- Executam uma ação expecífica
- Sempre deve haver `()` após invocar o método 
- O valor dentro dos parenteses chama-se "**argumento**"
- Também podem ser armazenadas em variáveis

Ex.:
```
const result = nomeCompleto.toLowerCase()

console.log(nomeCompleto.toUpperCase())
console.log(result)
```
**Output:**
> LEONARDO GONSALEZ

> leonardo gonsalez

- Deve-se notar que esses métodos não modificam o valor original



# Existem métodos que esperam um valor dentro dos parenteses:

## indexOf()

```
const index = nomeCompleto.indexOf("L")
console.log(index)
```

**Output:**
>0
- Este método busca um caractere expecificado e retorna a sua posição dentro da string 
- O caractere "L" está na posição 0 dentro da variável nomeCompleto

## lastIndexOf()
- retorna a posição da ultima ocorrencia de um caractere expecificado

Ex.:
```
const ultimaOcorrencia = nomeCompleto.lastIndexOf("a")
console.log(ultimaOcorrencia)
```

**Output:**
> 13

## slice()
- Retorna uma string recortada de acordo com os argumentos inseridos
- O primeiro argumento significa: "a partir de qual posição a string deve ser recortada?"
- O segundo argumento significa: "até qual posição a string deve ser recortada?"
- Retorna os caracteres entre as posições inseridas

Ex.:
```
const recortarString = nomeCompleto.slice(0, 7)
console.log(recortarString)
```

**Output:**
>Leonardo

## replace()
- Substitui um caractere ou sequência de caracteres por outros
- Não modifica a string original

```
const replaceString1 = nomeCompleto.replace("Leonardo", "Bernardo")
const replaceString2 = nomeCompleto.replace("o", "p")
console.log(replaceString1)
console.log(replaceString2)
```

**Output:**
>Bernardo Gonsalez

>Lepnardo Gonsalez

- Nota-se que apenas o primeiro caractere é substituido, enquanto o outro continua intacto