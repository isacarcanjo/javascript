# Array

## 1. Unshift

Add in the first position

```javascript
const array = [1, 2, 3];
array.unshift(0); // [ 0, 1, 2, 3 ]
```

## 2. Push

Add in the last position

```javascript
const array = [1, 2, 3];
array.push(0); // [ 0, 1, 2, 3 ]
```

## 3. Shift

Remove the first position

```javascript
const array = [1, 2, 3];
array.shift(); // [ 1, 2 ]
```

## 4. Pop

Remove the last position

```javascript
const array = [1, 2, 3];
array.pop(); // [ 1, 2 ]
```

## 5. Slice

Getting part of array

```javascript
const array = [1, 2, 3];
//      start, end
array.slice(0, 2); // [ 1, 2 ]
```

## 6. Splice

3 arguments
`index`,
`deleteCount`,
`list of elements to insert(optional)`

Removes elements by count from start

```javascript
var array = [1, 2, 3, 4, 5];
array = array.splice(2); // [ 3, 4, 5 ]
```

You can use to remove specific item from array

```javascript
var array = [1, 2, 3, 4, 5];
array.splice(2, 1); // [ 1, 2, 4, 5 ]
```

## 7. Some

Return true if there is only element or more that is accepted by conditional

```javascript
const array = [1, 2, 3, 4, 5];
const condi = (element) => element % 2 === 0; // true
```

## 8. Every

Return true if all elements is accepted by conditional

```javascript
const array = [1, 2, 3, 4, 5];
const condi = (element) => element < 20; // true
```

## 9. Find

Return first found element

```javascript
const array = [1, 2, 3, 4, 5];
const found = array.find((element) => element > 4); // 5
```

## 10. Index Of

Return first occurrence index found from array

```javascript
const array = [1, 2, 3, 4, 2];
const found = array.indexOf(2); // 1
```

## 11. Last Index Of

Return last occurrence index found from array

```javascript
const array = [1, 2, 3, 4, 2];
const found = array.lastIndexOf(2); // 4
```

## 12. Reverse

Reverse the list order

```javascript
const array = [1, 2, 3];
const reverse = array.reverse(); // [ 3, 2, 1 ]
```

## 13. Sort

Reverse the list order

```javascript
var fruit = ["cherries", "apples", "bananas"];
fruit.sort(); // ['apples', 'bananas', 'cherries']
```

## 14. Reduce

Reverse the list order

```javascript
const array = [1, 2, 3, 4];
const reduce = array.reduce((items, item) => {
  if (item < 2) return items; // Similiar continue
  items.push(item * 10);
  return items;
}, []); // [ 20, 30, 40 ]
```

## 15. Concat

Merge two arrays and return a new

```javascript
const array = [1, 2, 3];
const array2 = [4, 5, 6];
const merge = array.concat(array2); // [ 1, 2, 3, 4, 5, 6 ]
```

# Object

## 1. Entries

Return a array with key and values separated

```javascript
var obj = { foo: 'bar', baz: 42 };
console.log(Object.entries(obj)); // [ ['foo', 'bar'], ['baz', 42] ]
```

## 2. Freeze

Freeze the object, is not possible changes keys and values

```javascript
var obj = { text: 'aloha' };
Object.freeze(obj);
obj.text = "test"
console.log(obj) // { text: 'aloha' }
```

## 3. Has Own / Has Own Property

Check the object has the property specified, return true or false 

```javascript
var obj = { text: 'aloha' };
console.log(Object.hasOwn(obj, 'text')); // true
//or
console.log(obj.hasOwnProperty('text')); // true

```
