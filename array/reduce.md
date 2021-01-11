### The reduce() method reduces the array to a single value.
### phương thức reduce() giảm 1 mảng thành 1 giá trị đơn
ứng dụng để tính tổng , tích , hiệu , thương của 1 mảng ...  
gấp đôi 1 mảng ...   

### https://www.w3schools.com/jsref/jsref_reduce.asp
```
var numbers = [12,4,3,33,11,67,120];

function getSum(total, num, indexArray, arrOrigin) {
  return total + num;
}

function myFunction(item) {
  document.getElementById("demo").innerHTML = numbers.reduce(getSum, 0);
}
```


```
var numbers = [12,4,3,33,11,67,120];

function myFunction(item) {
  document.getElementById("demo").innerHTML = numbers.reduce(
    function (total, num, indexArray, arrOrigin) {
      return total + num;
    }, 0);
}
```


```
var numbers = [12,4,3,33,11,67,120];

function myFunction(item) {
  document.getElementById("demo").innerHTML = numbers.reduce(
    (total, num, indexArray, arrOrigin) => {
      return total + num;
    }, 0);
}
```




```
var numbers = [12,4,3,33,11,67,120];

function myFunction(item) {
  document.getElementById("demo").innerHTML = numbers.reduce(
    (total, num, indexArray, arrOrigin) => total + num; , 0);  
}
```

