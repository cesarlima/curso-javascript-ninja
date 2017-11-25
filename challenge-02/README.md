# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
somar(num1, num2){
  return num1 + num2;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var resultado = somar(3, 2);
resultado += 5;

// Qual o valor atualizado dessa variável?
10

// Declare uma nova variável, sem valor.
var variavel;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function adicionarValorAVariavel(){
  variavel = 15;
  return 'O valor da variável agora é ' + variavel;
}

// Invoque a função criada acima.
adicionarValorAVariavel();

// Qual o retorno da função? (Use comentários de bloco).
/*
  O valor da variável agora é 15
*/

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function calcular(num1, num2, num3){
  if(num1 === undefined || num2 === undefined || num3 === undefined) {
    return 'reencha todos os valores corretamente!';;
  } 

  return (num1 * num2 * num3) + 2;
}

// Invoque a função criada acima, passando só dois números como argumento.
calcular(2,5);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// Preencha todos os valores corretamente!

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
calcular(2, 5, 8);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
//82

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function tentarCalcular(num1, num2, num3){
  if(num1 === undefined && num2 === undefined && num3 === undefined){
    return false;
  } else if(num1 !== undefined && num2 === undefined && num3 === undefined) {
    return num1;
  } else if(num1 !== undefined && num2 !== undefined && num3 === undefined) {
    return num1 + num2;
  } else if(num1 !== undefined && num2 !== undefined && num3 !== undefined) {
    return (num1 + num2) / num3;
  } else {
    return null;
  }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
tentarCalcular(); //false

tentarCalcular(3); // 3

tentarCalcular(3, 5); // 8

tentarCalcular(3, 5, 2); // 4

tentarCalcular(null); // null
```
