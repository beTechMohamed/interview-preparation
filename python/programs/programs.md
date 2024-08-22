## Flatten Array
### a = [1,2,3,[4,5,6],[7,[8,9]]]

```bash
def flatten(array,index,output):
    if(index>=len(array)):
        return output
    if(type(array[index])==list):
        flatten(array[index],0,output)
    else:
        output.append(array[index])
    return flatten(array,index+1,output)
print(flatten(a,0,[]))
```

