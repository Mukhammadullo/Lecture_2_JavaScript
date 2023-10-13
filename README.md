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


