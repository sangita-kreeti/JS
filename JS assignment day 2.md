Topic: Scope, Hoisting, Control Structures, Regex, Numbers

# 1. If we execute this Javascript, what will the browser's console show?

```js

var text = 'outside';
function logIt(){
    console.log(text);
    var text = 'inside';
};
logIt();
```

Ans: 

The output will be undefiend because of When the logIt() function is called, the JavaScript interpreter first searches for a local variable called text within the function scope. Since text is declared with the var keyword inside the logIt() function, its declaration is hoisted to the top of the function, but the initialization of text to the string value 'inside' remains in place. Therefore, the value of text is undefined.

# 2. Write a regular expression  to reverse the first and last name.


```js
const name = prompt("Enter your name: ");
const reversedName = name.replace(/^(\w+)\s+(\w+)$/, "$2 $1");
console.log("Reverse: "+reversedName);

```


# 3. Write a Regular expression to validate email address.


# 4. Find the Output
```js
var x = 100;
console.log(x);   
function test()
{
    var x = 250;
    console.log(x);     
    if (x > 100)
    {
        let x = 350;
        console.log(x);
    }
    console.log(x);
}     
test();
console.log(x);
```
Ans:

The output will be
```
100
250
350
250
100
```
# 5. What is the difference of output between these two expressions? Give your reasons for it:
```js
a. 12 == “12”
b. 12 === “12”
c. Number(12) === 12
```
Ans: 

a. 12 == "12" compares the values of 12 and "12", and returns *true* because they have the same numerical value.

b. 12 === "12" compares the values and types of 12 and "12", and returns *false* because they have different types (12 is a number, and "12" is a string).

c. The expression Number(12) === 12 will return true.
Because of Number(12) will return the numerical value 12 and 12 is already a number.
For 12 === 12 comparison also both operands have the same type and value. 
That's why umber(12) === 12 will return true.

# 6. What is NaN?

NaN stands for "Not a Number" and is a special value in JavaScript. It is used to represent a value that is not a valid number.

```js
y="hello";
console.log(isNaN(y));

//output: true
```
Here "hello" is not a number that's why the return value is true.

```js
y=10;
console.log(isNaN(y))

//output: false
```
Here 10 is a number that's why the return value is false.

```js
if(NaN!=NaN)
{
    console.log("hello")
}
//output: hello
```
In JavaScript, NaN is not equal to any value, including itself. That's why the expression NaN != NaN evaluates to true.
