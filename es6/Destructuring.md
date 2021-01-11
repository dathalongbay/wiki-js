```
var data = $('body').data(), // data has properties house and mouse
  house = data.house,
  mouse = data.mouse
  ```
Một ví dụ khác của phép gán destructuring (từ Node.js):
```
var jsonMiddleware = require('body-parser').json

var body = req.body, // body has username and password
  username = body.username,
  password = body.password  
  ```
Trong ES6, chúng ta có thể thay thế code ES5 với các câu lệnh:
```
var {house, mouse} = $('body').data() // we'll get house and mouse variables

var {jsonMiddleware} = require('body-parser')

var {username, password} = req.body
```
Điều này cũng làm việc với mảng:
```
var [col1, col2]  = $('.column'),
  [line1, line2, line3, , line5] = file.split('\n')
  ```
