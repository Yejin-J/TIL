# โญObject   
## ๐Object ์์ฑ๊ณผ ํธ์ถ   
โ**์ฃผ์ํ  ์ **   
- ํ๋กํผํฐ๋ฅผ ๋ง๋ค ๋๋ `:` ์ฝ๋ก ์ ์ฌ์ฉํ๋ค.
- ์ด์ด์ ์๋ก์ด ํ๋กํผํฐ๋ฅผ ๋ง๋ค ๋๋ `,` ์ผํ๋ฅผ ์ฌ์ฉํ๋ค. `;`์ ํจ์๋ ๊ฐ์ฒด๊ฐ ๋๋  ๋ ์ฌ์ฉํ๋ค. 
  
โ **๊ฐ์ฒด ํธ์ถ ๋ฐฉ๋ฒ**
- ๋ฐฉ๋ฒ1, `๊ฐ์ฒด์ด๋ฆ.ํ๋กํผํฐ`
- ๋ฐฉ๋ฒ2, `๊ฐ์ฒด์ด๋ฆ["ํ๋กํผํฐ"]`   
```jsx
const playerName = 'yejin';
const playerPoints = 10;
const playerParty = false;

const player = {
  name : "yejin",
  points : 10,
  party : false,
}
console.log(player.name); // yejin
console.log(player["name"]); // yejin
```

## ๐Object ์๋ฐ์ดํธ
- `๊ฐ์ฒด์ด๋ฆ.์์ฑํ  ํ๋กํผํฐ` ์ ๊ฐ์ ํ ๋นํ๋ค. ๊ทธ๋ผ ์์ฑ๋๋ค.   
- โ **const๋ก ๊ฐ์ฒด๋ฅผ ์์ฑํ๋ฉด ๊ฐ์ ๋ณ๊ฒฝํ์ง ๋ชปํ๋๊ฑฐ ์๋๊ฐ์?**   
โ ์ฌ๊ธฐ์ ๊ฐ์ด ๋ณ๊ฒฝ๋ ๊ฑด `player`์ ํ๋กํผํฐ `party`์ ๊ฐ์ด์ง `player`์ ๊ฐ์ด ์๋๋ค. `const`์ ๊ฐ์ `player`์ด๋ค.

```jsx
player.party = true;
console.log(player.party); // true
```

## ๐Object ์ฐ์ฐ
- Object์ ํ๋กํผํฐ ๊ฐ์ ์ฐ์ฐํ๋ ๊ฒ ๊ฐ๋ฅํ๋ค.    
```jsx
player.points = player.points + 35;
console.log(player.points); //45
```
   
***
# ๐Object ํ์ฉ - ๊ณ์ฐ๊ธฐ ๋ง๋ค๊ธฐ   
```jsx
const calculator = {
  add : function(a, b){
    return a + b;
  },
  minus : function(a, b){
    return a - b;
  },
  multi : function(a, b){
    return a * b;
  },
  div : function(a, b){
    return a / b;
  },
  power : function(a, b){
    return a ** b;
  },
}
const add = calculator.add(522, 255);
const minus = calculator.minus(522, 255);
const multi = calculator.multi(5, 10);
const div = calculator.div(5, 10);
const power = calculator.power(2, 3);
```
