# Patika.dev Javascript Saat ve Karşılama

Yapmış olduğum bu projede "prompt" ile alınan bilginin kullanımını ve sürekli değişen bir yapının saat üzerinde gösterimini sağladık.

```javascript
//İsim
let isim = prompt("İsminiz:");
document.getElementById("karsilama").innerText = `Hoşgeldiniz, ${isim}..`;
//Saat
setInterval(() => {
  let time = new Date();
  let saat = time.toLocaleString("tr-TR", {
    year: "numeric",
    month: "long",
    day: "numeric",
    hour: "numeric",
    minute: "numeric",
    second: "numeric",
    hour12: false,
  });
  document.getElementById("saat").innerText = `${saat}`;
}, 500);
```

Sayfada kullanılan CSS kütüphanesi için: [Bulma.io](bulma.io)
