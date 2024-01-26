<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Scientific Calculator</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    #calculator {
      border: 2px solid #ccc;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    input {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      font-size: 16px;
    }

    button {
      width: 48px;
      height: 48px;
      font-size: 16px;
      margin: 5px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div id="calculator">
    <input type="text" id="display" readonly>
    <br>
    <button onclick="appendToDisplay('1')">1</button>
    <button onclick="appendToDisplay('2')">2</button>
    <button onclick="appendToDisplay('3')">3</button>
    <button onclick="clearDisplay()">C</button>
    <br>
    <button onclick="appendToDisplay('4')">4</button>
    <button onclick="appendToDisplay('5')">5</button>
    <button onclick="appendToDisplay('6')">6</button>
    <button onclick="operate('+')">+</button>
    <br>
    <button onclick="appendToDisplay('7')">7</button>
    <button onclick="appendToDisplay('8')">8</button>
    <button onclick="appendToDisplay('9')">9</button>
    <button onclick="operate('-')">-</button>
    <br>
    <button onclick="appendToDisplay('0')">0</button>
    <button onclick="operate('*')">*</button>
    <button onclick="operate('/')">/</button>
    <button onclick="calculateSquareRoot()">√</button>
    <br>
    <button onclick="appendToDisplay('.')">.</button>
    <button onclick="calculateExponent()">^</button>
    <button onclick="calculateResult()">=</button>
    <button onclick="calculateSin()">sin</button>
    <br>
    <button onclick="calculateCos()">cos</button>
    <button onclick="calculateTan()">tan</button>
    <button onclick="calculateLog()">log</button>
    <button onclick="calculateLn()">ln</button>
    <br>
    <button onclick="appendToDisplay('Math.PI')">π</button>
    <button onclick="appendToDisplay('Math.E')">e</button>
  </div>

  <script>
    function appendToDisplay(value) {
      document.getElementById('display').value += value;
    }

    function clearDisplay() {
      document.getElementById('display').value = '';
    }

    function operate(operator) {
      document.getElementById('display').value += operator;
    }

    function calculateSquareRoot() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = Math.sqrt(eval(value));
    }

    function calculateExponent() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = eval(value) ** 2;
    }

    function calculateResult() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = eval(value);
    }

    function calculateSin() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = Math.sin(eval(value));
    }

    function calculateCos() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = Math.cos(eval(value));
    }

    function calculateTan() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = Math.tan(eval(value));
    }

    function calculateLog() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = Math.log10(eval(value));
    }

    function calculateLn() {
      let value = document.getElementById('display').value;
      document.getElementById('display').value = Math.log(eval(value));
    }
  </script>
</body>
</html>
