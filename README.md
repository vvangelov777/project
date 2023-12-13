<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Simple Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="calculator">
        <input type="text" id="display" disabled>
        <div class="keys">
            <button>7</button>
            <button>8</button>
            <button>9</button>
            <button>+</button>
            <button>4</button>
            <button>5</button>
            <button>6</button>
            <button>-</button>
            <button>1</button>
            <button>2</button>
            <button>3</button>
            <button>*</button>
            <button>0</button>
            <button>C</button>
            <button>=</button>
            <button>/</button>
        </div>body {
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

    </div>
</body>
</html>
