<!DOCTYPE html>
<html>
<head>
    <title>Calculator</title>
    <style>
        .calculator {
            width: 200px;
            background-color: #f2f2f2;
            padding: 10px;
            border-radius: 10px;
            box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.2);
            margin: 0 auto;
        }
        input {
            width: 90%;
            padding: 10px;
            margin-bottom: 10px;
        }
        button {
            width: 50%;
            padding: 10px;
            background-color: #4CAF50;
            border: none;
            color: white;
            cursor: pointer;
        }
        button:hover {
            opacity: 0.8;
        }
        .output {
            font-weight: bold;
            text-align: right;
        }
    </style>
</head>
<body>
    <div class="calculator">
        <input type="text" id="value1" placeholder="">
        <input type="text" id="value2" placeholder="">
        <div class="output" id="result"></div>
        <button onclick="add()">+</button>
        <button onclick="subtract()">-</button>
        <button onclick="multiply()">*</button>
        <button onclick="divide()">/</button>
    </div>
    <script>
        function add() {
            var value1 = parseFloat(document.getElementById("value1").value);
            var value2 = parseFloat(document.getElementById("value2").value);
            var result = value1 + value2;
            document.getElementById("result").innerHTML = "Result: " + result;
        }
        function subtract() {
            var value1 = parseFloat(document.getElementById("value1").value);
            var value2 = parseFloat(document.getElementById("value2").value);
            var result = value1 - value2;
            document.getElementById("result").innerHTML = "Result: " + result;
        }
        function multiply() {
            var value1 = parseFloat(document.getElementById("value1").value);
            var value2 = parseFloat(document.getElementById("value2").value);
            var result = value1 * value2;
            document.getElementById("result").innerHTML = "Result: " + result;
        }
		function divide() {
            var value1 = parseFloat(document.getElementById("value1").value);
            var value2 = parseFloat(document.getElementById("value2").value);
            var result = value1 / value2;
            document.getElementById("result").innerHTML = "Result: " + result; 
		}
    </script>
</body>
</html>
