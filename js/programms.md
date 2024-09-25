### Flatten Array

```bash
let a = [1,2,3,[4,5,6],[7,[8,9]]]

const flatten = (array, index, output)=>{
    if (index>=array.length){
        return output;
    }
    if (Array.isArray(array[index])){
        flatten(array[index],0,output)
    }
    else{
        output.push(array[index])
    }
    return flatten(array,index+1,output)
}

console.log(flatten(a,0,[]))

```

```bash 
let students = [{id:1,name:"Moahmed"},{id:2,name:"Yasin"}, {id:1,name:"Moahmed"},{id:2,name:"Yasin"}, {id:3,name:"Srikanth"}];

let visited  = []
result = students.filter((item)=>{
  	const id = item["id"];
	if(!visited.includes(id)){
        visited.push(id);
    	return item;
    }
})

console.log(result)
```


Question-1

let arr1 = [1, 2, 2, 3, 4, 5, 5]; // size = n

let arr2 = [2, 4, 4, 6, 8, 10, 10]; // size = n

Requirements:

1. Find the numbers which are not common to two arrays

2. Solution should run in O(n) time complexity

Output 1,3,5,6,8,10

Questions

if request is made to t2 and then t1 Will the t1 return or it will be blocked by t2 ? Please explain why?

To Consider:

Pls consider node js core concepts like event loop, io vs cpu task 

const express = require('express');

const app = express();

const port = 3000;

app.get('/t1', (req, res) => {

    res.send('Hello World!');

});

app.get('/t2', (req, res) => {

    let c = 0;

    for (let i = 0; i < 10000000000; i++) {

        c++;

    }

    res.send('count ' + c);

});

app.listen(port, () => {

    console.log(`Example app listening on port ${port}`);

});

console.log(result);

Questions 3

Please create a program that can detect two strings are anagrams of each other!

Example: 

listen = silent

race = care

Requirements:

Solution should run in O(n) time complexity

Question 4

Create "two number sum problem solving"

Given array [3, 5, 8, 11, 1, -1, 7] and targetSum = 10

Output: [11,-1], [3,7]

 
