### Default Parameters in ES6
 Chúng ta có các câu lệnh để định nghĩa các tham số mặc định:
```
var link = function (height, color, url) {
    var height = height || 50
    var color = color || 'red'
    var url = url || 'http://azat.co'
    ...
}
```
  
  
```
var link = function(height = 50, color = 'red', url = 'http://azat.co') {
  ...
}
```
