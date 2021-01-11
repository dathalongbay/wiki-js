### Definition and Usage  
### https://www.w3schools.com/jsref/jsref_find.asp
The find() method returns the value of the first element in an array that pass a test (provided as a function).  
trả về 1 giá trị đầu tiên nếu phần tử đó pass qua test  
nếu ko tìm được thì trả về undefined  
```
var ages = [3, 10, 18, 20];

function checkAdult(age) {
  return age >= 18;
}

function myFunction() {
  document.getElementById("demo").innerHTML = ages.find(checkAdult);
}
```

