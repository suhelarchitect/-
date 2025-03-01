# -// script.js
const jokes = [
    "چۆن دەڵێن بەراز لە کاتی خەوتندا؟ - خەو بەراز!",
    "چۆن دەڵێن ماسی لە کاتی خەوتندا؟ - خەو ماسی!",
    "چۆن دەڵێن پشیلە لە کاتی خەوتندا؟ - خەو پشیلە!",
    "چۆن دەڵێن سەگ لە کاتی خەوتندا؟ - خەو سەگ!",
    "چۆن دەڵێن مرۆڤ لە کاتی خەوتندا؟ - خەو مرۆڤ!",
];

const jokeElement = document.getElementById("joke");
const jokeBtn = document.getElementById("jokeBtn");

jokeBtn.addEventListener("click", () => {
    const randomJoke = jokes[Math.floor(Math.random() * jokes.length)];
    jokeElement.textContent = randomJoke;
});
