# Classes
> fornece uma maneira mais estruturada e limpa de trabalhar com objetos com encapsulamento, herança...

## ***Construtor***
> Inicializar o estado inicial do Objeto

```
Class Product {
    constructor(name, price){
        this.name = name,
        this.price = price;
    }
}
```

## ***Métodos***
> funções que estão associadas a objetos ou classes e podem ser invocados para executar determinadas operações sobre esses objetos.

```
displayProduct(){
        console.log(`Product: ${this.name}`);
        console.log(`Price: $${this.price}`);
    }

calculateTotal(salesTax){
        return this.price + (this.price * salesTax);
    }
```

## ***Classe completa com seus métodos***

```
class Product {
    constructor(name, price){
        this.name = name,
        this.price = price;
    }

    displayProduct(){
        console.log(`Product: ${this.name}`);
        console.log(`Price: $${this.price}`);
    }

    calculateTotal(salesTax){
        return this.price + (this.price * salesTax);
    }
}

const salesTax = 0.05;

const product1 = new Product("Celular", 1000);

product1.displayProduct();                          //Saida: Product: Celular  Price: 1000

const total = product1.calculateTotal(salesTax);
console.log(`Total Price with Tax: $${total}`);     //Saída: Total Price with Tax: $1050
```

## ***Static***
> keyword que define propriedades ou métodos de uma classe que pertencem a classe em si,
sem a necessidade de instanciar um objeto.

```
class MathUtil{
    static PI =  3.14159;

    static getDiameter(radius){
        return radius * 2;
    }

    static getCircumference(radius){
        return 2 * this.PI * radius;
    }
}

console.log(MathUtil.PI)
console.log(MathUtil.getDiameter(10));
console.log(MathUtil.getCircumference(5))

class User{
    
    static userCount = 0;

    constructor(username){
        this.username = username;
        User.userCount++;
    }
}

const user1 = new User("Pedro");
const user2 =  new User("Sasa");
console.log(user1.username);
console.log(User.userCount);
```
