<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spider-Man Gwen Stacy Valentine</title>
    <style>
        body {
            font-family: 'Arial Rounded MT Bold', cursive, sans-serif; /* Cute and playful font */
            background-color: #ffcccc; /* Light pink background color */
            text-align: center;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container {
            max-width: 600px;
            padding: 20px;
            border-radius: 20px;
            background-color: rgba(255, 255, 255, 0.9);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: #ff007f; /* Pink text color */
        }

        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            background-color: #ff7f50;
            color: white;
            cursor: pointer;
            border-radius: 20px; /* Rounded corners */
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.1); /* Softer shadow */
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #ff6347;
        }

        img {
            width: 200px; /* Adjust as needed */
            height: auto;
            border-radius: 50%; /* heart shaped images */
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Softer shadow */
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Will you be my Valentine?</h1>
        <div id="message"></div>
        <div>
            <button onclick="chooseOption('Yes')">Yes</button>
            <button onclick="chooseOption('No')" id="noButton">No</button>
        </div>
    </div>

    <script>
        function chooseOption(option) {
            var messageDiv = document.getElementById('message');
            if (option === 'Yes') {
                messageDiv.innerHTML = "<p>Thank you my love, I can’t wait to spend this special day with you.☺️Iloveyou</p><img src='gifff.gif' alt='Happy Gwen Stacy'>";
            } else {
                var noButton = document.getElementById('noButton');
                var newX = Math.floor(Math.random() * (window.innerWidth - 200));
                var newY = Math.floor(Math.random() * (window.innerHeight - 200));
                noButton.style.position = 'absolute';
                noButton.style.left = newX + 'px';
                noButton.style.top = newY + 'px';
                messageDiv.innerHTML = "<p>Why not?😠 Please reconsider!!!</p><img src='angrygwen.gif.GIF' alt='Angry Gwen Stacy'>";
            }
        }
    </script>
</body>
</html>
