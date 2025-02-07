<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Goal Tracker</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 20px;
        }
        .tracker-container {
            display: inline-flex;
            align-items: center;
            background: #e0f2f1;
            padding: 10px;
            border-radius: 10px;
            border: 2px solid #4caf50;
        }
        .progress-container {
            width: 150px;
            height: 20px;
            background: #c8e6c9;
            border-radius: 10px;
            overflow: hidden;
            margin: 0 10px;
            position: relative;
        }
        .progress-bar {
            height: 100%;
            width: 0%;
            background: #4caf50;
            transition: width 0.3s ease-in-out;
        }
        button {
            background: #4caf50;
            color: white;
            border: none;
            padding: 5px 10px;
            margin: 0 5px;
            cursor: pointer;
            border-radius: 5px;
            font-size: 16px;
        }
        button:disabled {
            background: #ccc;
        }
    </style>
</head>
<body>
    <div class="tracker-container">
        <span style="font-size: 24px;">🌳</span>
        <button onclick="decreaseProgress()">-</button>
        <div class="progress-container">
            <div class="progress-bar" id="progressBar"></div>
        </div>
        <button onclick="increaseProgress()">+</button>
    </div>
    <p id="progressText">0%</p>

    <script>
        let progress = 0;

        function increaseProgress() {
            if (progress < 100) {
                progress += 10;
                updateProgress();
            }
        }

        function decreaseProgress() {
            if (progress > 0) {
                progress -= 10;
                updateProgress();
            }
        }

        function updateProgress() {
            document.getElementById("progressBar").style.width = progress + "%";
            document.getElementById("progressText").innerText = progress + "%";
        }
    </script>
</body>
</html>
