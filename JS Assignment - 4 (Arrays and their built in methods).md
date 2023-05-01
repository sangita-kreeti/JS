# 1. Given a string “Azad Ram Madiha Yash”. Return a string with the first letter of every word from the string. (Use built in methods).

```js
let str = "Azad Ram Madiha Yash";
let words = str.split(" ");
let result = words.map(word => word.charAt(0)).join("");

console.log(result); 

// Output: "ARMY"

```

# 2. Given an array [1, -4, 12, 0, -3, 29, -150]. Calculate the sum of all positive numbers (use built in array methods).

```js
const arr = [1, -4, 12, 0, -3, 29, -150];
const sumOfPositives = arr.reduce((acc, curr) => {
  if (curr > 0) {
    return acc + curr;
  } else {
    return acc;
  }
}, 0);

console.log(sumOfPositives); 

// Output: 42
```


# 3. Given an array [1, 2, 3, 4, 5]. Create a new array with the square of each element(use built in array methods).

```js
const array = [1, 2, 3, 4, 5];
const squaredArray =array.map((num) => num ** 2);
console.log(squaredArray);

// Output: [1, 4, 9, 16, 25]

```

# 4. Given an array [{ id: 2100, name: 'President Jacqueline' }, { id: 2114, name: 'Vice-president James' }, { id: 3016, name: 'House-captain Otis' },  { id: 4818, name: 'Prefect Finneas' }]. Create an array containing just the id of every individual. (write two solution one using iterator and another using built-in method)

```js
const array = [{ id: 2100, name: 'President Jacqueline' }, { id: 2114, name: 'Vice-president James' }, { id: 3016, name: 'House-captain Otis' }, { id: 4818, name: 'Prefect Finneas' }];

const idArray = array.map((obj) => obj.id);

console.log(idArray);

// Output: [2100, 2114, 3016, 4818]

```
