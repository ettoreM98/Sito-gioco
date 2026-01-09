<!DOCTYPE html>    
<html lang="it">    
<head>    
<meta charset="UTF-8">    
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>regalo del mio mori mori</title>    
    
<style>    
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap');    
    
body{    
    margin:0;    
    background:radial-gradient(circle,#0b1d17,#000);    
    font-family:'Orbitron',sans-serif;    
    color:#fff;    
    display:flex;    
    justify-content:center;    
    align-items:center;    
    min-height:100vh;    
}    
    
.container{    
    width:90%;    
    max-width:650px;    
    background:rgba(0,0,0,0.9);    
    border:2px solid #ff0055;    
    border-radius:15px;    
    padding:25px;    
    box-shadow:0 0 30px #ff0055;    
}    
    
h1,h2{text-align:center;color:#ff0055;}    
    
.timer{    
    text-align:center;    
    font-size:22px;    
    margin-bottom:15px;    
    color:#00ffcc;    
}    
    
input,button{    
    width:100%;    
    padding:12px;    
    margin:10px 0;    
    border-radius:6px;    
    border:none;    
    font-family:'Orbitron',sans-serif;    
    box-sizing: border-box; /* Aggiunto per evitare sbordamenti su mobile */  
}    
    
input{    
    background:#111;    
    color:#fff;    
    border:1px solid #ff0055;    
}    
    
button{    
    background:#ff0055;    
    color:#fff;    
    cursor:pointer;    
    font-weight: bold;  
}    
    
.answer{    
    background:#111;    
    padding:12px;    
    margin:8px 0;    
    border-radius:6px;    
    cursor:pointer;    
    border:1px solid #333;    
}    
    
.answer.selected{    
    background:#0f8a3a;    
    box-shadow:0 0 10px #0f8a3a;    
}    
    
.hidden{display:none;}    
    
.result img{    
    max-width:100%;    
    border-radius:10px;    
    margin-top:20px;    
    box-shadow:0 0 25px #ff0055;    
}    
</style>    
</head>    
    
<body>    
    
<div class="container">    
    
<div id="login">    
<h1>ACCESSO RISERVATO</h1>    
<input id="user" placeholder="Email" type="text">    
<input id="pass" type="password" placeholder="Password">    
<button onclick="checkLogin()">ENTRA NEL GIOCO</button>    
</div>    
    
<div id="rules" class="hidden">    
<p>    
Buongiorno concorrente numero 010 le regole del seguente gioco sono molto semplici.<br><br>    
Verrà sottoposta a un quiz su delle semplicissime domande di cultura generale.<br>    
Se le risposte corrette saranno 6 su 10 avrà accesso al suo regalo.<br><br>    
In caso contrario visto che c’è stato da poco il suo compleanno può scegliere se vedere per l’ultima volta un quadrato un triangolo o un cerchio.<br><br>    
Se ha capito la citazione può proseguire col quiz cliccando sul tasto start altrimenti può chiudere tutto qui e andare a casa.<br><br>    
(Prima però accompagni il suo fantastico magnifico e inimitabile fidanzato ettore dall’avvocato grazie )    
</p>    
<button onclick="startQuiz()">START</button>    
</div>    
    
<div id="quiz" class="hidden">    
<div class="timer" id="timerDisplay">05:00</div>    
<div id="quizContent"></div>  
</div>    
    
<div id="final" class="hidden">    
<h2>GRATTA E VINCI</h2>    
<button onclick="showResult()">GRATTA</button>    
<div id="result" class="result"></div>    
</div>    
    
</div>    
    
<script>    
const questions=[    
{q:"Quante sono le Sfere del Drago (quelle classiche)?",a:["7 quelle della Terra + 8 quelle di Namek","1","4","7"],c:3},    
{q:"Qual è il sogno di Luffy?",a:["Trovare tutti i frutti","Diventare il Re dei Pirati","Diventare famoso","Pirata più forte"],c:1},    
{q:"Takemichi può tornare nel passato grazie a:",a:["Un sogno","Un telefono","Una stretta di mano","Un pugno"],c:2},    
{q:"Chi è il fratello di Goku?",a:["Bardack","Gohan","Raditz","Vegeta"],c:2},    
{q:"Chi usa principalmente le spade?",a:["Usopp","Zoro","Sanji","Luffy"],c:1},    
{q:"Chi è Mikey?",a:["Il protagonista","Il più alto","Il leader della Tokyo Manji Gang","Il più intelligente"],c:2},    
{q:"Come si chiama l’attacco più famoso di Goku?",a:["Final Flash","Genkidama","Big Bang","Kamehameha"],c:3},    
{q:"Che tipo di pirata è Luffy?",a:["Solitario","Ex marinaio","Capitano Cappello di Paglia","Grande nave"],c:2},    
{q:"Cosa vuole fare Takemichi tornando nel passato?",a:["Vendicarsi","Salvare Hinata","Cambiare scuola","Capo gang"],c:1},    
{q:"Quale NON è un anime?",a:["Naruto Shippuden: Il videogioco","One Piece","Dragon Ball","Tokyo Revengers"],c:0}    
];    
    
let score=0,current=0,time=300,timerInterval;    
    
// Funzione rinominata per evitare conflitti  
function checkLogin(){    
    const userInput = document.getElementById("user").value;  
    const passInput = document.getElementById("pass").value;  
      
    if(userInput === "regalotardi" && passInput === "shein"){    
        document.getElementById("login").classList.add("hidden");    
        document.getElementById("rules").classList.remove("hidden");    
    } else {  
        alert("ACCESSO NEGATO");    
    }  
}    
    
function startQuiz(){    
    document.getElementById("rules").classList.add("hidden");    
    document.getElementById("quiz").classList.remove("hidden");    
    startTimer();    
    loadQuestion();    
}    
    
function startTimer(){    
    const timerDisplay = document.getElementById("timerDisplay");  
    timerInterval=setInterval(()=>{    
        time--;    
        let m=String(Math.floor(time/60)).padStart(2,'0');    
        let s=String(time%60).padStart(2,'0');    
        timerDisplay.innerText=`${m}:${s}`;    
        if(time<=0){    
            clearInterval(timerInterval);    
            endQuiz();    
        }    
    },1000);    
}    
    
function loadQuestion(){    
    if(current>=questions.length){endQuiz();return;}    
    const q=questions[current];    
    const quizDiv = document.getElementById("quiz");  
      
    // Puliamo il contenuto precedente mantenendo il timer  
    const timerHTML = document.getElementById("timerDisplay").outerHTML;  
    quizDiv.innerHTML = timerHTML + `<h2>${current+1}) ${q.q}</h2>`;  
      
    q.a.forEach((ans,i)=>{    
        let d=document.createElement("div");    
        d.className="answer";    
        d.innerText=ans;    
        d.onclick=()=>selectAnswer(d,i);    
        quizDiv.appendChild(d);    
    });    
}    
    
function selectAnswer(el,i){    
    el.classList.add("selected");    
    // Disabilita altri click  
    const allAnswers = document.querySelectorAll('.answer');  
    allAnswers.forEach(a => a.style.pointerEvents = 'none');  
  
    if(i===questions[current].c) score++;    
      
    setTimeout(()=>{  
        current++;  
        loadQuestion();  
    },600);    
}    
    
function endQuiz(){    
    clearInterval(timerInterval);    
    document.getElementById("quiz").classList.add("hidden");    
    document.getElementById("final").classList.remove("hidden");    
}    
    
function showResult(){    
    const resultDiv = document.getElementById("result");  
    if(score>=6){    
        resultDiv.innerHTML=`<h2>ACCESSO CONSENTITO</h2>    
        <img src="https://i.imgur.com/8RkR5QK.png">    
        <p style="text-align:center; font-size:18px; margin-top:10px;">iPad A16 rosa</p>`;    
    }else{    
        resultDiv.innerHTML=`<h2>ELIMINATO</h2>    
        <img src="https://i.imgur.com/7cMZKQm.png">`;    
    }    
}    
</script>    
    
</body>    
</html>  
