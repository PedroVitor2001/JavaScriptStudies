# Objetos
> Uma coleção de propriedades e/ou métodos relacionados que podem representar objetos do mundo real (pessoas, produtos, lugares...)

## ***Exemplo***:

```
const person1 = {

    firstName: "Spongebob",
    lastName: "Squarepants",
    age: 30,
    isEmployed: true,
    sayHello: function(){return "Hi, Im Spongebob"},
    eat: function(){return "Im eating a Krabby Patty"}

}

const person2 = {

    firstName: "Patrick",
    lastName: "Star",
    age: 42,
    isEmployed: false,
    sayHello: () => {return "Hi, Im Patrick"},
    eat: () => {return "Im eating Krabby Patty"} 

}

```

## ***Utilizando propriedades e funções***:

>Todas de uma vez:

```
console.log(person2.firstName, 
            person2.lastName,
            person2.age,
            person2.isEmployed,
            person2.eat()
            person2.sayHello());
```

> Uma por vez:

```
console.log(person1.firstName);
console.log(person1.lastName);
console.log(person1.age);
console.log(person1.isEmployed);
console.log(person1.eat());
console.log(person1.sayHello());

```

## ***.this***:
> referência ao objeto onde .this é usado (person.name = this.name)

> Não pode ser usado com Arrow function

```
const person1 = {

    firstName: "Spongebob",
    lastName: "Squarepants",
    age: 30,
    isEmployed: true,
    sayHello: function(){
        console.log(`Hi, im ${this.firstName}`)
    }
}
person1.sayHello();
```

