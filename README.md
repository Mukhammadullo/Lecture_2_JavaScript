## _1.What is Sciope in JavaScript?_
>### In JavaScript, the scope refers to the visibility and accessibility of variables, functions, and objects in a particular part of your code. It determines where these entities can be accessed and used.

_JavaScript has the following kinds of scopes:_
>_1.Global Scope-The default scope for all code running in script mode._
```js
let name="Muhammadullo";
let age=20;
let job="Student";

console.log(name);
console.log(age);
console.log(job);
```
>_2.Function Scope-The scope created with a function._
```js
function sumTwoNum(){
    
    //Function Scope
    let one=2;
    let two=3;
    return one+two;
}
console.log(sumTwoNum()) //5 
```
>_3.Block Scope in JavaScript-This scope restricts the variable that is declared  inside a specific block, from access by the outside of the block._
```js
if(true){
   let name="Muhammadullo"
   console.log(name)     
}
console.log(name)
```        
>_4.Module Scope- The scope for code running in module mode_

# _2.What is Hosting in JavaScipt_
>### Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution
```js
                           //In variables
//Let
console.log(num);
let num=23;
//Cannot access 'num' before initialization

//Const
console.log(number);
const number(12)

//Cannot access 'num' before initialization
//This event TDZ -Temporial Dead Zone   

//Var
console.log(number)
var number=123;
// undefined

            //In functions
//function declaration            
console.log(simple())
function simple(){
let number=23;
return number
}
// 23


//function Expression
_#arrow_

console.log(number)
let number=()=>{
let num=23
return num
//Cannot access 'number' before initialization

-#aynonimus-
console.log(number())
let number=function(){
let num=23
return num
}
}

-#IIFE-
(function () {
    let num = 23
    console.log(num);
})() //  Can not use it!


```
# _3.What is Recursion in JavaScipt?_
>### Recursion is when a function calls itself until someone stops it. If no one stops it then it'll 
recurse (call itself) forever. Recursive functions let you perform a unit of work multiple times.
Рекурсивная функция - это функция, которая вызывает сама себя внутри своего тела.
```js
function factorial(n) {
  if (n <= 1) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}

console.log(factorial(5)); // 120
```
# _4.What is Closure in JavaScript?_
>### A closure is the combination of a function bundled together (enclosed) with references to 
its surrounding state (the lexical environment). In other words, a closure gives you 
access to an outer function's scope from an inner function.
>## Замыкание — это набор функций, сгруппированных по ссылке.
его окружение (лексическое окружение). Другими словами, это дает вам завершение
получить доступ к области внешней функции из внутренней функции.
```js
let main = (one) => {
    return (two) => {
        return (three) => {
            return (four) => {
                return (five) => {
                    return (six) => {
                        return one + two + three + four + five + six 
                    }
                }
            }
        }
    }
}
console.log(main(1)(2)(3)(4)(5)(6));
```





