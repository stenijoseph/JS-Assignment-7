
## 1.Write short notes on below array methods with code examples.

## • reverse():-The reverse() method of Array instances reverses an array in place and returns the reference to the same array, the first array element now becoming the last, and the last array element becoming the first. In other words, elements order in the array will be turned towards the direction opposite to that previously stated.
## ex:-
```js
let nums=[1,2,3,4,5]
console.log(nums.reverse());                                         
```

## • sort():-The sort() method of Array instances sorts the elements of an array in place and returns the reference to the same array, now sorted. The default sort order is ascending, built upon converting the elements into strings, then comparing their sequences of UTF-16 code units values.
## ex:-
```js
let arr=["steni","binsi","anu"]
 console.log(arr.sort());
```

## • fill():-The fill() method of Array instances changes all elements within a range of indices in an array to a static value. It returns the modified array.
## ex:-
```js
let arr=[1,2,3,4,5,6]
console.log(arr.fill("a"));
```

## • filter():-The filter() method of Array instances creates a shallow copy of a portion of a given array, filtered down to just the elements from the given array that pass the test implemented by the provided function.
## ex:-
```js
let arr=[1,2,3,4,5]
let ans=arr.filter((item)=>{
    return item<4
 })
console.log(an s);
```

## • some():-The some() method of Array instances tests whether at least one element in the array passes the test implemented by the provided function. It returns true if, in the array, it finds an element for which the provided function returns true; otherwise it returns false. It doesn't modify the array.
## ex:-
```js
let isEven=(num)=>{
  return num%2===0
}
let arr=[1,2,3,4,5]
let ans=arr.some(isEven)
console.log(ans);
```

## • every():-The every() method of Array instances tests whether all elements in the array pass the test implemented by the provided function. It returns a Boolean value.
## ex:-
```js
let arr=[1,2,3,4,5]
 let ans=arr.every((item)=>{
   return item>0
 })
console.log(ans);
```

## • map():-The map() method of Array instances creates a new array populated with the results of calling a provided function on every element in the calling array.
## ex:-
```js 
let arr=[1,2,3,4,5]
let ans=arr.map((item)=>{
   return item*4
})
 console.log(ans);
```

## • forEach():-The forEach() method of Array instances executes a provided function once for each array element.
## ex:-
```js
const array1 = ['a', 'b', 'c'];
array1.forEach((element) => console.log(element));
```

## • reduce():-The reduce() method of Array instances executes a user-supplied "reducer" callback function on each element of the array, in order, passing in the return value from the calculation on the preceding element. The final result of running the reducer across all elements of the array is a single value.
## ex:-
```js
const arr=[150,10,3]
 const myFunction=(total,num)=>{
    return total-num
 }
 const output=arr.reduce(myFunction)
 console.log(output);
 ```

## • indexOf():-The indexOf() method of Array instances returns the first index at which a given element can be found in the array, or -1 if it is not present.
```js
let arr=["steni","saliha"]
console.log(arr.indexOf("steni"));
```

## 2.write a function that takes an array of numbers as an argument and returns the sum of its elements.

```js
let arr=[150,10,5,10,20]
let myFunction=(total,num)=>{
    return total+num
}
let output=arr.reduce(myFunction)
console.log(output)
```


## 3.Create a function that filters strings in an array by their length.

```js
let arr=["apple","mango","orange","pineapple","banana"]
let filteredArr=arr.filter((str)=>
   str.length>5
    
)
console.log(filteredArr)
```
 
## 4.Create a function that returns a new array containing the square roots of each number in the original array [1,4,9,16,25](Math.sqrt())

```js
let numbers=[3,8,9,34,50]
let result=numbers.map((num)=>{
   return Math.sqrt(num)
})
console.log(result);
```

## 5. Write a function that prints the number 1 to 100. But for multiples of 3, print Fizz instead of the number, and for multiples of 5, print Buzz. For the numbers that are multiples of both 3 and 5, print FizzBuzz(write the code in the browser’s snippet and invoke the function inside the console)

```js
let count=1
let outPut=[]
let counter=()=>{
    if(count%3 == 0 && count%5==0){
      outPut.push("FizzBuzz")  
    }
    else if(count%3==0){
        outPut.push("Fizz")
    }
    else if(count%5==0){
        outPut.push("Buzz")
    }
    else {
        outPut.push(count)
    }
    
    count++
    console.log(outPut)
}
counter()
```