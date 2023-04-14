# JS assignment
## Topics: Data types, variables, and Strings

1. Write a program that declares a variable using var, let, and const and prints the value to the console.

   Ans: 
    ```js
    var x;
    let y;
    const z=3;
    console.log(x);
    console.log(y);
    console.log(z);
    ```
2. Write a program that reassigns a value to a variable declared with let and prints the new value to the console.
    
    Ans: 
    ```
    let m_name='Sangita';
    m_name='Adak';
    console.log(m_name)
    ```

3. Write a program that tries to reassign a value to a variable declared with const and prints the message to the console.

    Ans: 
    ```
    const m_name='Sangita';
    m_name='Adak';
    console.log(m_name)
    ```
    ```
    Output::

    m_name='Adak';
      ^
    TypeError: Assignment to constant variable.
    ```
    *We can't reassign value of a constant.*
    <br><br>

4. Write a program to declare a const, let, var variable within an if statement and try to access the variable outside the if block, what is the result?

    Ans: 
    ```
    if (NaN!=NaN)
    {
        var x;
        let y;
        const z=3;
    }
    console.log(x);
    console.log(y);
    console.log(z);
    ```
     ```
    Output::

    undefined
    console.log(y);
                ^
    ReferenceError: y is not defined
    ```

    *In JavaScript, the scope of a variable declared with const or let is block-scoped, which means that it is only accessible within the block in which it is declared. If we try to access a const or let variable from outside its block, you will get an error.*
    <br><br>

5. Write a program that concatenates two or more strings and prints the result to the console.

    Ans: 
    ```
    let str1 = "We ";
    let str2 = "are ";
    let str3 = "Indian";
    console.log(str1.concat(str2,str3))
    ```


6. Write a program that takes a string as input and prints the length of the string to the console.

    Ans: 
    ```
    let m_name = prompt("Please the string:");
    console.log("Length:" +m_name.length);
    ```

    

7. Write a program that converts a string to uppercase and prints the result to the console.

    Ans: 
    ```
    let m_name = prompt("Please the string in lowercase:");
    console.log("Uppercase:" +m_name.toUpperCase());
    ```

    
