```js
Array.prototype.unshift() 
```
Insert into the beginning of an array. Must call on variable otherwise it will return the length of array
```js
//arr will be 4 (length of array)
let arr = [4,5,6].unshift(3);
//arr2 will be [3,4,5,6]
let arr2 = [4,5,6];
arr2.unshift(3);
```