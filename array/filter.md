### ví dụ array.filter()
```
var ages = [32, 33, 16, 40];

function checkAdult(age) {
  return age >= 18;
}

function myFunction() {
  document.getElementById("demo").innerHTML = ages.filter(checkAdult);
}
```
```
var ages = [32,33,16,40];

function checkAdult(){
  return age >= 18;
}

function myFunction() {
  document.getElementById("demo").innerHTML = ages.filter(checkAdult);
}
```
### sử dụng callback
```
var ages = [32,33,16,40];
function myFunction() {
  document.getElementById("demo").innerHTML = ages.filter(function(){
    return age >= 18;
  });
}
```
### sử dụng arrow function
```
var ages = [32,33,16,40];
function myFunction() {
  document.getElementById("demo").innerHTML = ages.filter(() => {
    return age >= 18;
  });
}
```

```
var ages = [32,33,16,40];
function myFunction() {
  document.getElementById("demo").innerHTML = ages.filter(() => return age >= 18; );
}
```



