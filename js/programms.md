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
