# reminder\<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Message for You</title>
    <style>
        body {
            background-color: hwb(1 78% 5%);
            font-family: 'cursive', cursive;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }

        .container {
            background-color: hwb(0 63% 18%);
            border: 2px solid #e63946;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            position: relative;
        }

        .title {
            font-size: 36px;
            color: #e63946;
            margin-bottom: 20px;
        }

        .message {
            font-size: 20px;
            color: #333;
            margin-bottom: 20px;
        }

        .button {
            background-color: #e63946;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 20px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .button:hover {
            background-color: #d62839;
        }

        .hidden-message {
            display: none;
            font-size: 22px;
            color: #333;
            margin-top: 20px;
            animation: fadeIn 1s;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .heart {
            display: inline-block;
            width: 20px;
            height: 20px;
            background-color: rgb(235, 31, 31);
            position: relative;
            margin-left: 5px;
            transform: rotate(-45deg);
        }

        .heart::before,
        .heart::after {
            content: '';
            width: 20px;
            height: 20px;
            background-color: rgb(235, 31, 31);
            border-radius: 50%;
            position: absolute;
        }

        .heart::before {
            top: -15px;
            left: 0;
        }

        .heart::after {
            left: 15px;
            top: 0;
        }
    </style>
</head>
<body><i>
    <div class="container">
        <h1 class="title">  Quick reminder for My Baby</h1>
        <p class="message">Hey love! i Just wanted to remind you...</p>
        <button class="button" onclick="showMessage()">touch this heart like you touched mine ❤️</button>
        <p class="hidden-message" id="hiddenMessage">i love you more than i can say in words baby ..  
           i love you more than warm blankets in winter ....More than snow loves chiku...more than getting my favorite chocolates in cramps 
          I love you sooo much! <span class="heart"></span></p>
    </div>

    <script>
        function showMessage() {
            document.getElementById('hiddenMessage').style.display = 'block';
        }
    </script>
</body><i>
</html>
