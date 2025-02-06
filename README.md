<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffccd5;
            margin: 0;
            padding: 50px;
        }
        h1 {
            color: #d6336c;
        }
        .heart {
            font-size: 50px;
        }
        .buttons {
            margin-top: 20px;
        }
        .btn {
            font-size: 20px;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            margin: 10px;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff4d6d;
            color: white;
        }
        .no {
            background-color: #6c757d;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>Will You Be My Valentine? <span class="heart">❤️</span></h1>
    <div class="buttons">
        <button class="btn yes" onclick="alert('YOU HAD NO CHOICE! I love you! ❤️')">Yes</button>
        <button class="btn no" id="noButton">No</button>
    </div>

    <script>
        const noButton = document.getElementById("noButton");

        noButton.addEventListener("mouseover", () => {
            const x = Math.random() * (window.innerWidth - 100);
            const y = Math.random() * (window.innerHeight - 50);
            noButton.style.left = `${x}px`;
            noButton.style.top = `${y}px`;
        });

        noButton.addEventListener("click", () => {
            alert("You can't say no! 😜");
        });
    </script>
</body>
</html>
