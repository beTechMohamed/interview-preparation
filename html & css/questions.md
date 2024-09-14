### center the div inside div.
```bash 
body {
  margin: 20px;
}

.outter{
  width:500px;
  height:500px;
  background-color:red;
  display:flex;
  justify-content:center; /* for horizontal scale*/
  align-items:center; /* for vertical scale*/
}

.inner{
 width:25px;
 height:25px;
 background-color:blue;
}
  
<div class="outter">
    <div class="inner">
    </div>
</div>
```