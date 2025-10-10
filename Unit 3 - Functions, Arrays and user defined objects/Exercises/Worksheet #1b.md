# Arrow functions

## 1. Two arguments

Transform this function:
```js
function sum(num1, num2){
    return num1 + num2
}

sum(40,2)
sum(42,0)
console.log("the answer to everything is", sum(42,0))
```

<details><summary>ANSWER - CLICK ME!</summary>

This is a possible answer:

```js
const sum = (num1, num2) => num1+num2
```
You need parenthesis around the arguments because there are more than one.
You don't need curly brackets or the `return` keyword because arrow functions give you an implicit return. 

However, this is also okay:
```js
const sum = (num1, num2) => {return num1+num2}
```

You can also use `let` but in that case your variable could be redefined later (which may cause bugs).
</details>

***

## 2. One argument

Transform this function that tells you how long a string is:

```js
function stringLength(str){
    console.log(`the length of "${str}" is:`, str.length)
}

let longestCityNameInTheWorld = "Taumatawhakatangihangakoauauotamateaturipukakapikimaungahoronukupokaiwhenuakitanatahu"

stringLength(longestCityNameInTheWorld)
```

<details><summary>ANSWER - CLICK ME!</summary>

This is a possible answer:

```js
const stringLength = str => console.log(`the length of "${str}" is:`, str.length)
```

Here you don't need parenthesis aroung the argument because it's just one (but you could have the parenthesis, no difference). 
You don't need curly brackets because it's just one line.
</details>

***

## 3. One argument, pt.2

Let's change the previous function a bit to include a variable and a return statement:

```js
function stringLength(str){
    let length = str.length
    console.log(`the length of "${str}" is:`, length)
    return str.length
}

stringLength("willynilly")
```

***

## 4. One argument

Transform this function that selects a random element from the array and concatenates it to your name:

```js
let alerts = ["Hey, you are awesome", "You are so wonderful", "What a marvel you are", "You're so lovely", "You're so sweet that I'd think you're a sweet potato -- and I LOOOOVE POTATOES"]

function showAlert(name){    
    alert(alerts[(Math.floor(Math.random()*alerts.length))] + `, ${name}!`)
}

showAlert("you ball of fluff")
```

***

## 6. Write an arrow function that returns the string, Hello, I am ${name}, and I am ${age} years old.

***
## 7.  Write an arrow function that takes an array of integers, and returns the sum of the elements in the array. Google and use the built-in reduce array method for this.

***
## 8. The syntax of this function is wonky. Can you fix it to use the shortest arrow function possible?
```js
let eye = "eye";

const fire =
(

) =
>
{
 return `bulls-`;
}
```

***
## 9. Refactor the following ES5 function to use an arrow function:
```js
const fibonacci = function(n) {
if (n < 3) return 1;
return fibonacci(n - 1) + fibonacci(n - 2);
}
```
