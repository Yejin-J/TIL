# ๐ฅ Date ๊ฐ์ฒด๋ฅผ ํ์ฌ ์ฌ์ดํธ์ ์ ์ฉ

## ์ด๋ฒคํธ ์ข๋ฃ ํ์ด๋จธ ์์ฑ
์ด๋ฒคํธ ์ข๋ฃ ์๊ฐ์ "event-stamp.png" ์ด๋ฏธ์ง๊ฐ ํ๋ฉด์ ๋ฎ์ผ๋ฉด์ ์ข๋ฃ alert()์ด ์คํ๋๋ค.

HTML

```html
<div class="event-end" id="eventEnd">
   <img src="/event-stamp.png">
   <span></span>    
</div>
```

CSS

```css
.event-end{
	position: absolute; 
	width: 100%; 
	height: 100%; 
	background: rgba(0,0,0,0.8); 
	z-index: 111; 
	display:block;
}
.event-end > img{
	position: fixed; 
	top: 50%; 
	left: 50%; 
	transform: translate(-50%,-50%);
}
.event-end > span{
	width: 50px;
	height: 50px;
	position: fixed;
	right: 0;
	bottom: 0;
}
```

JavaScript

```jsx
<script>
    let nowDate = new Date();
    let endDate = new Date(2022,3,25,17,0,0,0);

    function viewEnd(mm){
      mm = nowDate > endDate;
      if(mm == true){
        document.getElementById('eventEnd').style.display = "block"
        alert('๋ง๊ฐ๋ ์ด๋ฒคํธ๋ก ํ์ฌ ํ์ด์ง ๋ด์์ ์ด๋ฒคํธ๊ฐ๋ก ๊ตฌ๋งค์ ๋์์์ด ํ๋ถ์ฒ๋ฆฌ๋  ์ ์์ต๋๋ค.');
      }else{
        document.getElementById('eventEnd').style.display = "none";
      }
    }
    viewEnd();
  </script>
```
