<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Request</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffe6e6;
            margin: 0;
        }
        .container {
            text-align: center;
            background-color: #ff99cc;
            padding: 40px;
            border-radius: 15px;
        }
        h1 {
            font-size: 2rem;
            color: #ff0066;
        }
        button {
            background-color: #ff0066;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2rem;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.2s ease;
        }
        button:hover {
            background-color: #cc0052;
        }
        #yesButton {
            display: inline-block;
        }
        #noButton {
            display: inline-block;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Will you be my Valentine's baby?</h1>
        <p>From Charles to Nicole</p>
        <button id="yesButton">Yes</button>
        <button id="noButton">No</button>
    </div>

    <script>
        let noButton = document.getElementById("noButton");
        let yesButton = document.getElementById("yesButton");
        let scale = 1; // Start with normal size

        noButton.addEventListener("click", function() {
            scale += 0.2; // Increase size by 0.2 each time
            yesButton.style.transform = "scale(" + scale + ")";
        });

        yesButton.addEventListener("click", function() {
            alert("Yey! Nicole said yes! I love you baby hehehe!");
        });
    </script>

</body>
</html>
