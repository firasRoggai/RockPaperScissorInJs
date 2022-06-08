const pcPick = document.getElementById('pc-pick')
const userPick = document.getElementById('user-pick')
const resultdisp = document.getElementById('result')
const possible = document.querySelectorAll('button')
const playerResult = document.querySelector('#playerResult')
const pcResult = document.querySelector('#pcResult')
const winner = document.querySelector('#winner')
let playerCounter = 0;
let pcCounter = 0;
function getResult(){
    if(pcchoice == userchoice){result = `It's a draw`;}
    else if(pcchoice == 'rock'&&userchoice == "sciccor" ||pcchoice == 'sciccor'&&userchoice == "paper"|| pcchoice == 'paper'&&userchoice == "rock"){
     result = 'You lost'
     pcCounter++
    }
    else{result = 'You won' 
    playerCounter++
}
    return result;
}
const list = ["rock","paper","sciccor"];
let result;
let userchoice;
let pcchoice;
let myimg = {
    rock:"./fist.png",
    paper:"./hello.png",
    sciccor:"./scissors.png"
}
// console.log(myimg["rock"])
possible.forEach(possible => possible.addEventListener('click',(e)=>{
    userchoice = e.target.id
    userPick.setAttribute('src',myimg[userchoice]) 
    pcchoice = list[generateComputer()];
    pcPick.setAttribute('src',myimg[pcchoice]) 
    resultdisp.textContent = getResult();
    playerResult.textContent = playerCounter + " ";
    pcResult.textContent = pcCounter;
    if(pcCounter == 4){winner.textContent = "الميكرو"}
    if(playerCounter == 4){winner.textContent="فراس و عدنان"}
}))

function generateComputer(){
    const randomNumber = Math.floor(Math.random() * 3)
    return randomNumber;

}
