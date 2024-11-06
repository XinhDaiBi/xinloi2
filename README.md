<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Xin Lỗi</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f2f2f2;
           background-size: contain;
        }
        #question {
            font-size: 24px;
            margin-bottom: 20px;
        }
        #button-container {
            display: flex;
            gap: 10px;
            justify-content: center;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
        h1{
            font-family: 'Courier New', Courier, monospace;
            color: pink;
            -webkit-text-stroke: 2px gray;
        }
        .special-font{
            font-family: 'Courier New', Courier, monospace;
            color: white;
        }
    </style>
</head>
<body background="image/z6004206228883_fc99dce55bc1f491badd0df07d4362a0.jpg">
    <div id="app">
        <div id="question"><h1>Cho Anh Xin Lỗi Được Hămmmmmmmm Péeeee </h1></div>
        <div id="button-container">
            <button id="noButton" onclick="moveButton()">Không</button>
            <button id="yesButton" onclick="nextQuestion()">Có</button>
        </div>
    </div>

    <script>
        function moveButton() {
            const noButton = document.getElementById("noButton");
            const randomX = Math.floor(Math.random() * 300) - 150;
            const randomY = Math.floor(Math.random() * 200) - 100;
            noButton.style.position = "relative";
            noButton.style.left = randomX + "px";
            noButton.style.top = randomY + "px";
        }

        function nextQuestion() {
            const question = document.getElementById("question");
            const yesButton = document.getElementById("yesButton");
            if (question.innerText === "Cho Anh Xin Lỗi Được Hămmmmmmmm Péeeee") {
                question.innerText = "Em có đi ăn bún đậu với anh không";
                question.classList.add("special-font");
            } else {
                question.innerText = "Anh Yêu Em";
                yesButton.style.display = "none";
                document.getElementById("noButton").style.display = "none";
                setTimeout(function() {
                    window.location.href = "https://mcdn.coolmate.me/image/April2023/meme-xin-loi-meme-meo-xin-loi-meme-xin-loi-duoc-chua-hai-huoc-vui-nhon-1566_963.jpg";
                }, 500);
            }
        }
    </script>
</body>
</html>

