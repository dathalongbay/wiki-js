
ví dụ 1 :  
sử dụng promise then()
```
fetch('coffee.jpg')
.then(response => {
  if (!response.ok) {
    throw new Error(`HTTP error! status: ${response.status}`);
  } else {
    return response.blob();
  }
})
.then(myBlob => {
  let objectURL = URL.createObjectURL(myBlob);
  let image = document.createElement('img');
  image.src = objectURL;
  document.body.appendChild(image);
})
.catch(e => {
  console.log('There has been a problem with your fetch operation: ' + e.message);
});
```
viết lại với async
```
async function myFetch() {
  try {
    let response = await fetch('coffee.jpg');

    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`);
    } else {
      let myBlob = await response.blob();
      let objectURL = URL.createObjectURL(myBlob);
      let image = document.createElement('img');
      image.src = objectURL;
      document.body.appendChild(image);
    }
  } catch(e) {
    console.log(e);
  }
}

myFetch();
```
ví dụ 2 : 
```
async function f() {
    console.log("---"); // "done!"
    let promise1 = new Promise((resolve, reject) => {
        setTimeout(() => resolve("done1!"), 5000)
    });
    let promise2 = new Promise((resolve, reject) => {
        setTimeout(() => resolve("done2!"), 3000)
    });
    let promise3 = new Promise((resolve, reject) => {
        setTimeout(() => resolve("done3!"), 1000)
    });

    let result1 = await promise1; // wait until the promise resolves (*)
    let result2 = await promise2; // wait until the promise resolves (*)
    let result3 = await promise3; // wait until the promise resolves (*)

    console.log(111); // "done!"
    console.log(result1); // "done!"
    console.log(222); // "done!"

    console.log(result2); // "done!"

    console.log(result3); // "done!"
}

f();
```
