### Features

- É só instalar e usar. Não requer configurações extras.

- Funciona tanto para v-text-field quanto input

- Extremamente leve

### Instalação


```js
npm install vuejs-money-br --save

import money from  'vuejs-money-br'
Vue.use(money)
```

### Uso

```html
<input  v-model="preco"  v-money />

-ou- 

<v-text-field  v-model="preco"  v-money />


Também é possível passar a quantidade de casas decimais como parâmetro utilizando a tag precision, como o exemplo abaixo:

<v-text-field  v-model="preco"  v-money="{ precision: 4 }" /> <!-- 4 casas decimais -->

Precision só aceita NÚMEROS INTEIROS maiores ou igual a 0 e menores que 6.
Caso qualquer outro valor seja passado, será utilizado 2 casas decimais.
```

## Propriedades

- O sufixo é R$

- Até 5 casas decimais utilizando a tag precision

- Ponto ( . ) separando os milhares

- Exemplo: R$ 47.210,55

## Thanks to:
- https://github.com/luizhenriquerdias/vuejs-money

- https://github.com/vuejs-tips/v-money

- https://github.com/lmarqs/v-money