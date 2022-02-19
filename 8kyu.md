# 8kyu tasks


## [Find numbers which are divisible by given number](https://www.codewars.com/kata/55edaba99da3a9c84000003b)
Complete the function which takes two arguments and returns all numbers which are divisible by the given divisor. First argument is an array of `numbers` and the second is the `divisor`.


## Example
```
divisibleBy([1, 2, 3, 4, 5, 6], 2) == [2, 4, 6]
```


## Solution
```javascript
function divisibleBy(numbers, divisor){
  let newArr = [];
  for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % divisor == 0) {
      newArr.push(numbers[i]);
    }
  }
  return newArr;
}
```


## [Double Char](https://www.codewars.com/kata/56b1f01c247c01db92000076)
Given a string, you have to return a string in which each character (case-sensitive) is repeated once.


```
doubleChar("String") ==> "SSttrriinngg"

doubleChar("Hello World") ==> "HHeelllloo  WWoorrlldd"

doubleChar("1234!_ ") ==> "11223344!!__  "
```
Good Luck!


## Solution
```javascript
function doubleChar(str) {
  let arr = str.split('');
  return arr.map((item) => item + item).join('');
}
```