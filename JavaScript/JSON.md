# JSON๊ณผ ๋ฉ์๋
### ๐JSON.stringify()
javaScript์ object, array ๋ฑ ์ด๋ค ๊ฒ์ด๋  ๋ฌธ์ํ์ผ๋ก ๋ฐ๊ฟ์ฃผ๋ ํจ์   
```jsx
const num = 1;
JSON.stringify(num); // "1"

const array = [1,2,3,4,5];
JSON.stringify(array); // "[1,2,3,4,5]"
```   

### ๐JSON.parse()
๋ฌธ์ํ์ผ๋ก ๋ณํ๋ ๊ฐ์ฒด๋ฅผ ๋ค์ ๊ฐ์ฒด๋ก ๋ง๋๋ ํจ์
```jsx
const strArray = JSON.stringify(array);
JSON.parse(strArray); // [1,2,3,4,5]
```
