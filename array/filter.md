### ví dụ array.filter()

### https://www.w3schools.com/jsref/jsref_filter.asp
Return an array of all the values in the ages array that are 18 or over:  

```
var ages = [32,33,16,40];

function checkAdult(age){
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
  document.getElementById("demo").innerHTML = ages.filter(function(age){
    return age >= 18;
  });
}
```
### sử dụng arrow function
```
var ages = [32,33,16,40];
function myFunction() {
  document.getElementById("demo").innerHTML = ages.filter((age) => {
    return age >= 18;
  });
}
```

```
var ages = [32,33,16,40];
function myFunction() {
  document.getElementById("demo").innerHTML = ages.filter((age) => return age >= 18; );
}
```

### Definition and Usage ( định nghĩa và cách dùng )
The filter() method creates an array filled with all array elements that pass a test (provided as a function).  
phương thức filter() tạo 1 mảng với các phần từ được truyền vào 1 hàm test ( nếu ok giá trị đó sẽ được truyền vào array mới ngược lại sẽ bỏ đi )  
Note: filter() does not execute the function for array elements without values.  
  
Note: filter() does not change the original array.  
Phương thức filter() này không thay đổi mảng gốc . 
   
ví dụ lọc bỏ các số lẻ :

```
var olds = [32,33,16,40];
function myFunction() {
  document.getElementById("demo").innerHTML = olds.filter((odd) => return ((odd % 2) == 0); );
}
```
    
```
var olds = [32,33,16,40];
function myFunction() {
  document.getElementById("demo").innerHTML = olds.filter(odd => ((odd % 2) == 0) );
}
```    
```
var olds = [32,33,16,40];
function myFunction() {
  let c = olds.filter(odd => ((odd % 2) == 0));
  
  console.log(c);
};

myFunction() ;
```


