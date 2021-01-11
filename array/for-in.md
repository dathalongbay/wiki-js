
duyệt object
```
var person = {fname:"John", lname:"Doe", age:25}; 
  
  var text = "";
  var x;
  for (x in person) {
    text += person[x] + " ";
  }
  document.getElementById("demo").innerHTML = text;
```

duyệt mảng
``` 
  var person = [1,2,3,4,5];
  
  var text = "";
  var x;
  for (x in person) {
    text += person[x] + " ";
  }
  document.getElementById("demo").innerHTML = text;
```
