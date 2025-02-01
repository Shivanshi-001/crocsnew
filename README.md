<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lychee Facts</title>
    <style>
        body {
            font-family: sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }

        .container {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            text-align: center;
        }

        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 15px;
        }

        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Lychee Fact</h1>
        <p id="fact-display">Click the button to see a fact</p>
        <button id="new-fact-button">Get New Fact</button>
    </div>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const factDisplay = document.getElementById('fact-display');
            const newFactButton = document.getElementById('new-fact-button');
            let facts = [];

            // Load the JSON file
            fetch('facts.json')
              .then(response => response.json())
              .then(data => {
                facts = data;
              })
            .catch(error => console.error('Error loading facts:', error));


            newFactButton.addEventListener('click', function() {
                if (facts.length === 0) {
                    factDisplay.textContent = "No facts available";
                    return;
                }
                const randomIndex = Math.floor(Math.random() * facts.length);
                factDisplay.textContent = facts[randomIndex].fact;
            });
        });
    </script>
</body>
</html>
