<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Online Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="calculator">
        <input type="text" id="display" readonly>
        <div class="keys">
            <button onclick="appendToDisplay('7')">7</button>
            <button onclick="appendToDisplay('8')">8</button>
            <button onclick="appendToDisplay('9')">9</button>
            <button onclick="appendToDisplay('+')">+</button>
            <button onclick="appendToDisplay('4')">4</button>
            <button onclick="appendToDisplay('5')">5</button>
            <button onclick="appendToDisplay('6')">6</button>
            <button onclick="appendToDisplay('-')">-</button>
            <button onclick="appendToDisplay('1')">1</button>
            <button onclick="appendToDisplay('2')">2</button>
            <button onclick="appendToDisplay('3')">3</button>
            <button onclick="appendToDisplay('*')">*</button>
            <button onclick="appendToDisplay('0')">0</button>
            <button onclick="clearDisplay()">C</button>
            <button onclick="calculate()">=</button>
            <button onclick="appendToDisplay('/')">/</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}

.calculator {
    border: 2px solid #333;
    border-radius: 5px;
    padding: 20px;
}

input[type="text"] {
    width: calc(100% - 40px);
    margin-bottom: 10px;
    padding: 10px;
    font-size: 18px;
}

.keys {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

button {
    padding: 15px;
    font-size: 18px;
    border-radius: 5px;
    border: none;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

button:hover {
    background-color: #ddd;
}
function appendToDisplay(value) {
    document.getElementById('display').value += value;
}

function clearDisplay() {
    document.getElementById('display').value = '';
}
