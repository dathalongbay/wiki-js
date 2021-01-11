# method map()
### https://www.w3schools.com/jsref/jsref_map.asp
## Definition and Usage
The map() method creates a new array with the results of calling a function for every array element.  
phương thức map() tạo 1 mảng với các phần tử trong mảng được trả về từ function được truyền vào trong phương thức map()  

The map() method calls the provided function once for each element in an array, in order.  

Note: map() does not execute the function for array elements without values.  

Note: this method does not change the original array.  

```
var numbers = [65, 44, 12, 4];
var newarray = numbers.map(myFunction)

function myFunction(num) {
  return num * 10;
}

document.getElementById("demo").innerHTML = newarray;
```

```
var numbers = [65, 44, 12, 4];
var newarray = numbers.map(function(num) {
  return num * 10;
});
```

```
var numbers = [65, 44, 12, 4];
var newarray = numbers.map(num => num * 10 );
```
