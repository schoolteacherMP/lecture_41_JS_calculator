`<!DOCTYPE html>
<html>
  <head>
    <title>Калькулятор</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
      }
      h1 {
        text-align: center;
      }
      input[type="number"] {
        padding: 10px;
        font-size: 16px;
        border: 1px solid #ccc;
        border-radius: 5px;
        margin-right: 10px;
      }
      button {
        padding: 10px;
        font-size: 16px;
        border: none;
        border-radius: 5px;
        background-color: #007bff;
        color: #fff;
        cursor: pointer;
      }
      button:hover {
        background-color: #0062cc;
      }
      input[type="number"][disabled] {
        background-color: #f8f9fa;
      }
    </style>
  </head>
  <body>
    <h1>Калькулятор</h1>
    <div style="text-align: center">
      <input type="number" id="num1" placeholder="Введите первое число">
      <input type="number" id="num2" placeholder="Введите второе число">
      <br><br>
      <button onclick="add()">+</button>
      <button onclick="subtract()">-</button>
      <button onclick="multiply()">*</button>
      <button onclick="divide()">/</button>
      <br><br>
      <input type="number" id="result" placeholder="Результат" disabled>
    </div>
    <script>
      function add() {
        let num1 = Number(document.getElementById("num1").value);
        let num2 = Number(document.getElementById("num2").value);
        let result = num1 + num2;
        document.getElementById("result").value = result;
      }

      function subtract() {
        let num1 = Number(document.getElementById("num1").value);
        let num2 = Number(document.getElementById("num2").value);
        let result = num1 - num2;
        document.getElementById("result").value = result;
      }

      function multiply() {
        let num1 = Number(document.getElementById("num1").value);
        let num2 = Number(document.getElementById("num2").value);
        let result = num1 * num2;
        document.getElementById("result").value = result;
      }

      function divide() {
        let num1 = Number(document.getElementById("num1").value);
        let num2 = Number(document.getElementById("num2").value);
        let result = num1 / num2;
        document.getElementById("result").value = result;
      }
    </script>
  </body>
</html>`
