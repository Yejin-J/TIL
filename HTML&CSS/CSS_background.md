# background
## ๐background-image
### gradient
- **์ ํ ๊ทธ๋ผ๋์ธํธ linear-gradient(direction, color1, color2, ...)**   
**direction** : to right, to bottom right, 0.5turn, 60deg ๋ฑ   
**repeating-linear-gradient()** : ์ ํ ๊ทธ๋ผ๋์ธํธ ๋ฐ๋ณต
[linear-gradient ์ฐธ๊ณ ](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Images/Using_CSS_gradients)
```CSS
/* ๊ธฐ๋ณธ */
background-image: linear-gradient(to right, blue, red); 

/* ํฌ๋ช๋ */
background-image: linear-gradient(60deg, white 10%, black 20%);
```


- **๋ฐฉ์ฌํ ๊ทธ๋ผ๋์ธํธ radial-gradient(shape size, color1, color2, ...)**   
**shape size** : circle(์ํ)   
**repeating-radial-gradient()** : ์ํ ๊ทธ๋ผ๋์ธํธ ๋ฐ๋ณต   
[radial-gradient ์ฐธ๊ณ ](https://www.w3schools.com/css/css3_gradients_radial.asp)
```CSS
background-image: radial-gradient(circle, red, yellow, green);
background-image: radial-gradient(red 10%, yellow 50%, green 90%);
/* ๊ฒ์ ์๋ ์๊น์ ์์ชฝ์ ์๋ ์๊น๋ณด๋ค %๊ฐ ๋์์ผ ํ๋ค. */
```

- **์๋ฟํ ๊ทธ๋ผ๋์ธํธ conic-gradient(color1, color2,...)**   
**repeating-conic-gradient()** : ์๋ฟํ ๊ทธ๋ผ๋์ธํธ ๋ฐ๋ณต     
[conic-gradient ์ฐธ๊ณ ](https://www.w3schools.com/css/css3_gradients_conic.asp)
```CSS
background-image: conic-gradient(red 10%, yellow 50%, green 90%);

/* red ์์ญ 0deg๋ถํฐ 180deg๊น์ง */
background-image: conic-gradient(red 0deg, red 180deg, yellow, green);

/* 90deg์์ ์์ */
background-image: conic-gradient(from 90deg, red 0deg, red 180deg, yellow, green);

/* ์ค์ฌ์์น๊ฐ 60% 70%๋ก ์ด๋ */
background-image: conic-gradient(at 60% 70%, red 0deg, red 180deg, yellow, green);
```
