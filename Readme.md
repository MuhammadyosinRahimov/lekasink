# Синхронизатсия код дар JavaScript чист?

## Sincxroni kod kode meboshad ki
## 1. Layn ba layn merava.


## 2. Vaqte ki da yagonjo ashibka shava prapuskat namekna.

## 3.Agar da yagonjo ashibka shava dalshe kod kor namekna.


const p = document.querySelector(".p");
p.innerHTML = "My name is Maruf"
alert("Text set !")
p.style.color = "red"

#  Что такое асинхронность код на JavaScript?


## Asincxroni kod kode meboshad ki 
 ## 1. Line ba lane merava.

 ## 2. Vaqte ki da yagonjo ashibka shava prapuskat mekna.

## 3.Agar da yagonjo ashibka shava dalshe kod kor mekna

const p = document.querySelector('.p');
setTimeout(() =>{
    p.innerHTML = "Hello, world!"
}, 5000);
p.style.color = "red";

# # 3 Tarzi nawishtani kodi Asincxroni vujud dorad.
## 1.Callbacks:
## 2.Promise:
## 3.async/await:


#  1. Asincxroni callbecks funksiyae meboshad, ki ba funksiya digar intiqol doda meshavad va baroi yagon korro ijro kardan oghoz mekunad.


fuction get(callback){
    setTimeout(( =>{
         calback("Hello world")
    },1000

    ))
    get fuction(value);
    console.log(value);
}

# 2. new Promise da JavaScript yak kansturkture meboshad ki xub idora kardani amalyoti asincxroni meboshad. On istifoda burda meshavad, ki oyo hamin amalyoti asincxroni bo muvaffaqiyat ijor meshavad yo ne.

let promise = new Promise((resolve, reject) => {
    // do something
})

let promise = new Promise((resolve, reject) => {
    if(10  > 11){
        return resolve("test is true")
    }
    return resolve("test is false")
});
console.log(promise
.then(() => console.log(response))
.catch(() => console.log(err))
0);

#  new Promise doroi 3 holat mebosh.
## 1.Pending -  Дар интизорӣ;
## 2.Fulfilled - Ичро шуд;
## 3.Rejected - Рад карда шуд;


# API chist ?
## API mexanizme meboshad ki ba du kampanent pragrama  imkon medihad ki muoshirat kunand.

## Api ho metavonand farq kunand.
## va az hama papulyarnii onho in RestApi meboshad.

# Rest Api chist?

## REST API (Интерфейси барномасозии барномаи интиқоли намояндагии давлатӣ) аст
## маҷмӯи қоидаҳо ва принсипҳо барои эҷоди хидматҳои веб, ки бо мубодилаи маълумот
## ҳамдигар. Он ба услуби меъмории REST асос ёфтааст, ки чӣ гуна муштариёнро муайян мекунад
## ва серверҳо бояд бо ҳамдигар муошират кунанд

# Fetch chist?

## Fetch ин функсия дар JavaScript муосир аст, ки барои қабули дархостҳои HTTP ба дурдаст истифода мешавад
## захираҳо ба монанди API ё серверҳо. Он роҳи оддӣ ва қулайи муоширатро фароҳам меорад
## бо шабака ва гирифтани маълумот аз Интернет.Бо истифода аз функсияи fetch (), шумо метавонед
## ирсол дархостҳои шабака ба сервер - ҳам қабул ва фиристодани маълумот. Усули а бар мегардонад
## ваъда бо объекти ҷавоб, ки дорои маълумоти иловагӣ (вазъияти посух,
## сарлавҳаҳо) ва ҷавоб ба дархост
fetch("https:// jsonplaceholder.tyicode.com/posts")\
.then((response) =>{
    response.json
})
```javascript
function fetchData(url){
    return new Promise((resolve,reject) =>){
        fetch(url)
        .then((response) => response.json){
        .then((data) => resolve(data))
        .catch((err) => reject(err))
        }
    }
}
fetchData("https://jsonplaceholder.tyicode.com")
.then((data) =>console.log(data))
.catch((err) => reject(err))