# JavaScript Annotations

##  ***Arrow Function***:
> As arrow functions oferecem uma sintaxe mais curta e sucinta em comparação com as funções tradicionais em JavaScript. Isso pode tornar o código mais legível e fácil de entender, especialmente para funções simples.

### ***Sem Arrow Function***:
```
const double = function(num) {
    return num * 2;
};
```

### ***Utilizando Arrow Funciton***:
```
const doublue = (num) => num * 2;
```

### ***Utilizando com Arrays***:
> Arrow functions são frequentemente usadas em métodos de array, como map, filter e reduce.

### ***.map() .filter() .reduce()***:
```
const numbers = const numbers = [1, 2, 3, 4, 5];

const cube = numbers.map((element) => Math.pow(element, 3));

const isEven = numbers.filter((element) => element % 2 == 0);

const total =  numbers.reduce((prev, next) => prev + next);
```

### ***.this***
> Em JavaScript, o valor de this em uma função depende de como a função é chamada.

### ***Objeto Pessoa***:
```
const pessoa = {
    nome: 'Sasa',
    irNaAcademia: function (){
        this.nome // funciona
    }
}

const pessoa = {
    nome: 'Sasa',
    irNaAcademia: () => {
        this.nome // não funciona: this é indefinido
    }
}


```
