<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Sir Piorque</title>
<style>
body{background:black;text-align:center;color:white;margin:0;overflow:hidden;font-family:Arial;padding:0}
h1{margin-top:25px;font-weight:100;font-size:26px;animation:wave 2s infinite,colorChange 2s infinite alternate}
@keyframes wave{0%,100%{transform:rotate(-1.5deg)}50%{transform:rotate(1.5deg)}}
@keyframes colorChange{0%{color:#00ccff;text-shadow:0 0 15px #00ccff}100%{color:#00ff99;text-shadow:0 0 15px #00ff99}}
.petal{position:fixed;top:-20px;font-size:22px;animation:fall linear forwards}
@keyframes fall{to{transform:translateY(110vh) rotate(360deg)}}
.side-flowers{position:fixed;top:50%;transform:translateY(-50%);display:flex;flex-direction:column;gap:15px}
.left{left:10px}.right{right:10px}
.tulip{font-size:32px}
.message{max-width:380px;margin:15px auto;font-weight:100;font-size:13px;line-height:20px;color:#ddd;background:rgba(255,255,255,0.05);padding:12px;border-radius:10px}
</style>
</head>
<body>

<div class="side-flowers left">
<div class="tulip">🌷</div>
<div class="tulip" style="filter:hue-rotate(90deg)">🌷</div>
<div class="tulip" style="filter:hue-rotate(180deg)">🌷</div>
<div class="tulip" style="filter:hue-rotate(270deg)">🌷</div>
</div>

<div class="side-flowers right">
<div class="tulip" style="filter:hue-rotate(45deg)">🌷</div>
<div class="tulip" style="filter:hue-rotate(135deg)">🌷</div>
<div class="tulip" style="filter:hue-rotate(225deg)">🌷</div>
<div class="tulip" style="filter:hue-rotate(300deg)">🌷</div>
</div>

<h1>Happy Teachers Day Sir!</h1>
<h1 style="font-size:19px;">Sir JOHN EZEKIEL ARCABAL PIORQUE</h1>

<div class="message">
Sir, thank you po talaga sa lahat. Sa pagtuturo po at sa pag-intindi samin kahit minsan po makulit kami.<br><br>
Naappreciate po namin yung effort nyo araw araw sir, kahit po pagod na kayo tinuturuan nyo pa din kami ng maayos. Kayo po yung teacher na di namin makakalimutan.<br><br>
Pasensya na po sir medyo simple lang po tong nagawa ko, first time ko lang po gumawa ng ganito. Pero pinaghirapan ko po talaga to para sa inyo.<br><br>
Happy Teachers Day po ulit sir! Ingat po kayo palagi sir!
</div>

<p style="font-size:11px;opacity:0.5;">- From your student</p>

<script>
function createPetal(){
var p=document.createElement("div");
p.className="petal";
p.innerHTML="🌸";
p.style.left=Math.random()*100+"%";
p.style.animationDuration=(Math.random()*1+2)+"s";
document.body.appendChild(p);
setTimeout(()=>{p.remove()},3000);
}
setInterval(createPetal,100);
</script>
</body>
</html>
