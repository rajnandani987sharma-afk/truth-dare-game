<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Truth or Dare</title>

<style>
body{
font-family: Arial;
background:#ff4d6d;
color:white;
text-align:center;
padding:40px;
}

.container{
background:white;
color:black;
padding:20px;
border-radius:10px;
max-width:400px;
margin:auto;
}

button{
padding:10px 20px;
margin:10px;
border:none;
border-radius:5px;
background:#ff4d6d;
color:white;
font-size:16px;
}

#result{
margin-top:20px;
font-size:18px;
font-weight:bold;
}
</style>

</head>
<body>

<div class="container">
<h2>Truth or Dare Game</h2>

<button onclick="getTruth()">Truth</button>
<button onclick="getDare()">Dare</button>

<p id="result">Click Truth or Dare</p>

</div>

<script>

const truths = [
"Apka biggest secret kya hai?",
"Kya aapka koi crush hai?",
"Kabhi jhoot bola hai parents se?",
"Sabse embarrassing moment kya tha?"
];

const dares = [
"10 pushups karo",
"Funny dance karo",
"Ek gaana gaao",
"Mirror ke saamne funny face banao"
];

function getTruth(){
let random = Math.floor(Math.random()*truths.length);
document.getElementById("result").innerText = truths[random];
}

function getDare(){
let random = Math.floor(Math.random()*dares.length);
document.getElementById("result").innerText = dares[random];
}

</script>

</body>
</html>
