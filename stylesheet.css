let firstCard=0;
let secondCard=0;
let card= 0;
let a = 0;
let total=0;
let playing = false;
let cardsEl = document.getElementById("cards-el")
let totalEl = document.getElementById("total-el")
let messageEl = document.getElementById("message-el")

function getRandomValue(){
    let a = Math.floor(Math.random()*13)+1
    if(a> 10){
        a=10
    }
    return a;
}

function startGame(){
    if(playing === false){
        reset()
        firstCard = getRandomValue()
        secondCard = getRandomValue()
        cardsEl.textContent += firstCard + " - " + secondCard
        total += firstCard + secondCard   
        totalEl.textContent += total;
        result()    
        playing = true  
                  
    }
    
}

function newCard(){
    if (playing === true){
        card = getRandomValue()
        cardsEl.textContent += " - " + card
        total += card
        totalEl.textContent = "Total: " + total
        result()
    }
    
}
function result(){
    if (total < 21){
        messageEl.textContent = "Another card?"
    } else if (total === 21){
       messageEl.textContent = "WINNER"
       document.getElementById("blackjack-msg").textContent = ""
       document.getElementById("blackjack-msg1").textContent = "BlackJack"
       playing = false

       

    } else {
            messageEl.textContent = "Try Again";
            playing = false
                

    }
}
function reset(){
    total = 0
    cardsEl.textContent="Cards: "
    totalEl.textContent="Total: "
    document.getElementById("blackjack-msg").textContent = "BlackJack"
    document.getElementById("blackjack-msg1").textContent = ""
    result()

}
