<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Syed Dhanisha 💙</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(180deg,#001233,#000814);
color:white;
text-align:center;
overflow-x:hidden;
min-height:100vh;
}

#loader{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:#000;
display:flex;
justify-content:center;
align-items:center;
font-size:35px;
z-index:9999;
}

.container{
padding:20px;
}

h1{
font-size:3rem;
margin-top:20px;
}

.date{
font-size:1.2rem;
margin-bottom:20px;
}

.gallery{
margin-top:20px;
}

.gallery img{
width:280px;
height:380px;
object-fit:cover;
border-radius:20px;
box-shadow:0 0 25px #00aaff;
}

.btn{
margin:10px;
padding:15px 25px;
border:none;
border-radius:15px;
cursor:pointer;
background:#00aaff;
color:white;
font-size:18px;
}

.message{
margin-top:30px;
font-size:20px;
padding:15px;
}

.heart{
position:fixed;
bottom:-50px;
font-size:24px;
animation:floatUp linear infinite;
pointer-events:none;
}

@keyframes floatUp{
0%{
transform:translateY(0);
opacity:1;
}
100%{
transform:translateY(-110vh);
opacity:0;
}
}

#cake{
display:none;
font-size:100px;
margin-top:20px;
animation:bounce 1s infinite;
}

@keyframes bounce{
0%,100%{
transform:translateY(0);
}
50%{
transform:translateY(-20px);
}
}

.countdown{
font-size:24px;
margin-top:10px;
}

.memoryBox{
display:none;
margin-top:20px;
padding:15px;
background:rgba(255,255,255,0.1);
border-radius:15px;
}

.footer{
margin-top:40px;
padding-bottom:20px;
}
</style>
</head>

<body>

<div id="loader">
💙 Loading Memories...
</div>

<div class="container">

<h1>🎂 Happy Birthday Syed Dhanisha 💙</h1>

<p class="date">23 June 2007 ✨</p>

<div class="countdown" id="countdown"></div>

<div class="gallery">
<img id="slide" src="photo1.jpg.jpeg">
</div>

<button class="btn" onclick="nextPhoto()">📸 Next Memory</button>

<button class="btn" onclick="showCake()">🎂 Cut Cake</button>

<button class="btn" onclick="showMemory()">💙 Open Message</button>

<div id="cake">
🎂
</div>

<div class="memoryBox" id="memoryBox">
<h2>💙 Special Message 💙</h2>
<p>
Happy Birthday Nishaaa Mahh🎉<br><br>

💙Happy birthday dee❤️ wifeyyyy life long happy 🥰ah iru enime ne Edhukum feel pannatha un kuda always na irupaa💋 pattu enna switch tion vandhalum 🧕unna vittu 🫰pogamatta chlow❤️‍🔥 nee eppomey happy irundha🥺 podhum pappu 😻unna eppomey 🥹sirika vechu pathukura 🫂💋nambalukulla 💞evaloo sanda 💚vandhalum nane💙 vandhu sorry 💜keppa chloow🖤 inmel na un kitta sanda poda Matta chloow idhu varaiyum romba sanda poturupa🤍 adhukula sorry ♥️pattu unna ennaku romba pudikum pappu maa💋 indha world la na romba pudichathu unna mattum dha chloomeyy 🫀nee ya life 💝varuvenu nanachi kuda 💜pakkala thangoow♥️ pattu romba thanks papa ya life vandhadhuku 😻chloow ennaku ellameyy nee mattum tha🥰enna nee romba care pandra pattu mah♾️ caring patner & una  💋romba miss pandra🧕 chloow olunga msg kuda panna mudiyala chlooww 🥺sorryy chlooww love you lots dee wifeyyyy once again happy Birthday dee wifeyyyy 💋 indha day nee happy iru patteyy Na😘 eppomey unna vittu pogamatta 🤭chloow nee feel pannadha😊 love you lots muu Kutty papa 💋Wish you a very Happy birthday my princess eapovume happy yaa eru edakum feel pana kudatha Unaku edathavathu onu na first unaku na vanthu irupa chlowww eapovume yenaku first priority nee tha nee matum so una edakagavm miss panida matan un happiness & sad renduthulayum na un kuda tha irupa so you don't worry i am always with you dee kutty papa & once again happy birthday dee wifeyyyy 💋🥰🫀💎🫂💯
</p>
</div>

<div class="message">
🌟 Every memory becomes special when shared with the right people 💙
</div>

<div class="footer">
This is for you dee papa 💙
</div>

</div>

<script>

setTimeout(()=>{
document.getElementById("loader").style.display="none";
},3000);

let photos=[
"photo1.jpg.jpeg",
"photo2.jpg.jpeg",
"photo3.jpg.jpeg",
"photo4,jpg.jpeg",
"photo5jpg.jpeg"
];

let index=0;

function nextPhoto(){
index++;
if(index>=photos.length){
index=0;
}
document.getElementById("slide").src=photos[index];
}

function showCake(){
document.getElementById("cake").style.display="block";
alert("🎉 Happy Birthday Nishaaa Maahh💙");
}

function showMemory(){
document.getElementById("memoryBox").style.display="block";
}

for(let i=0;i<80;i++){

let heart=document.createElement("div");

heart.classList.add("heart");

heart.innerHTML="💙";

heart.style.left=Math.random()*100+"%";

heart.style.fontSize=(15+Math.random()*25)+"px";

heart.style.animationDuration=(4+Math.random()*6)+"s";

heart.style.animationDelay=Math.random()*5+"s";

document.body.appendChild(heart);

}

function updateCountdown(){

const birthday=new Date("June 23, 2026 00:00:00").getTime();

const now=new Date().getTime();

const distance=birthday-now;

if(distance<0){

document.getElementById("countdown").innerHTML=
"🎉 Birthday Celebration Time 💙";

return;
}

const days=Math.floor(distance/(1000*60*60*24));

const hours=Math.floor(
(distance%(1000*60*60*24))
/
(1000*60*60)
);

const minutes=Math.floor(
(distance%(1000*60*60))
/
(1000*60)
);

const seconds=Math.floor(
(distance%(1000*60))
/
1000
);

document.getElementById("countdown").innerHTML=
"⏳ "+days+" Days "+
hours+" Hours "+
minutes+" Minutes "+
seconds+" Seconds";

}

setInterval(updateCountdown,1000);

updateCountdown();

</script>

</body>
</html>
