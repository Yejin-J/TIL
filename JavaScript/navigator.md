#πnavigator κ°μ²΄
λΈλΌμ°μ μ μ΄μμ²΄μ μ λν μ λ³΄λ₯Ό μ κ³΅νλ€.

## navigatore.geolocation
μΉμμ μ₯μΉμ μμΉλ₯Ό μμλΌ λ μ¬μ©

## navigatore.geolocation.getCurrentPosition(successFunc, errorFunc)
νμ¬ μμΉλ₯Ό κ°μ Έμ¨λ€.
- `successFunc` - λ¬Έμ μμ λ μ€νλλ ν¨μ (ex. μμΉ μ λ³΄ μ κ³΅μ λμνμ λ λ°μ)
- `errorFunc` - λ¬Έμ μμ λ μ€νλλ ν¨μ (ex. μμΉ μ λ³΄ μ κ³΅μ λμνμ§ μμμ λ λ°μ)   
```jsx
function onGeoOk(position){
  const lat = position.coords.latitude; //μλ
  const lon = position.coords.longitude; //κ²½λ
  alert(`your location ${lat}, ${lon}`);
}
function onGeoErroe(){
  alert("Can't find your location!");
}

navigatore.geolocation.getCurrentPosition(onGeoOk, onGeoErroe);
```   
