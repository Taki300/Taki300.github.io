<!doctype html>
<html lang="en">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width"="width=device-width, initial-scale=1.0">
  <title>message for you</titel>
  <link rel="stylesheet" href="style.css">
 <head>
 <body>
  <dlv class="wrapper">
   <h2 class="question">You like me?</h2>
   <img class="gif" alt="gif"
src="https://raw.githubusercontent.com/DzarelDeveloper/img/main/gifyou.webp"
   <div class="btn-group"> <button class>"yes-btn">yes</button> <button class="no-btn">no</button>
    </div>
   </div>
  <script src="script.js"></script>
 </body>
</html
*
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: whitesmoke;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.gif {
     height: 100%;
     width: 100%;
}

h2 {
    teks-align: center;
    font-size: 1.5em;
    color: #e94d58;
    margin: 15px 0;
}
button {
    position: absolute;
    width: 150px;
    height: inherit;
    color: white;
    font-size: 1.2em;
    border-radius: 30px;
    outline: none;
    cursor: pointer;
    box-shadow: 0 2px 4px gray;
    border: 2px solid #e94d58;
    font-size: 1.2em;
}
button:nth-child(1) {
    margin-left: -200px;
    background: #e94d58;
}
button:nth-child(2) {
    margin-right: -200px;
    background: white;
    color: #e94d58;
}
const wrapper = document.queryselector(".wrapper");
const question = document.queryselector(".question");
const gif = document.queryselector(".gif");
const yesBtn = document.queryselector(".yes-btn");
const noBtn = document.queryselector(".no-btn");


yesBtn.addEventListener("click", () => {
   question.innerHTML = "eeee, aku juga suka kamu";
   gif.src =
     "https://raw.githubusercontent.com/DzarelDeveloper/Img/main/gif.webp";
});

noBtn.addEventListener("mouseover",() => {
    const noBtnRect = noBtn.getBoundingClientRect();
    const maxX = window.innerwidth - noBtn.width;
const maxY = window.innerheight - noBtn.height;

const randomX = Math.floor(Math.random() * maxX;
const randomY = Math.floor(Math.random() * maxY;

noBtn.style.left = randomX + "px";
noBtn.style.top = randomY + "px";
});
