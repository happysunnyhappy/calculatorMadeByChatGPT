# calculatorMadeByChatGPT
<meta charset="utf-8">
<!DOCTYPE html>
<html>
<head>
	<title>网络计算器</title>
	<style>
		body {
			font-family: Arial, sans-serif;
			background-color: #f2f2f2;
		}
		
		.container {
			max-width: 400px;
			margin: 0 auto;
			padding: 20px;
			background-color: #fff;
			border-radius: 5px;
			box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
			text-align: center;
		}
		
		input[type="number"] {
			padding: 5px;
			margin: 5px;
			border-radius: 5px;
			border: none;
			background-color: #f2f2f2;
			width: 100%;
		}
		
		button {
			padding: 10px;
			margin: 5px;
			border-radius: 5px;
			border: none;
			background-color: #4CAF50;
			color: #fff;
			cursor: pointer;
			width: 100%;
			transition: background-color 0.3s ease;
		}
		
		button:hover {
			background-color: #3e8e41;
		}
	</style>
</head>
<body>
	<div class="container">
		<h1>网络计算器</h1>
		<label for="num1">数字1:</label>
		<input type="number" id="num1" name="num1">
		<label for="num2">数字2:</label>
		<input type="number" id="num2" name="num2">
		<br>
		<button onclick="add()">加</button>
		<button onclick="subtract()">减</button>
		<button onclick="multiply()">乘</button>
		<button onclick="divide()">除</button>
		<br>
		<label for="result">结果:</label>
		<input type="number" id="result" name="result" disabled>
	</div>
	
	<script>
		function add() {
			var num1 = parseInt(document.getElementById("num1").value);
			var num2 = parseInt(document.getElementById("num2").value);
			document.getElementById("result").value = num1 + num2;
		}
		
		function subtract() {
			var num1 = parseInt(document.getElementById("num1").value);
			var num2 = parseInt(document.getElementById("num2").value);
			document.getElementById("result").value = num1 - num2;
		}
		
		function multiply() {
			var num1 = parseInt(document.getElementById("num1").value);
			var num2 = parseInt(document.getElementById("num2").value);
			document.getElementById("result").value = num1 * num2;
		}
		
		function divide() {
			var num1 = parseInt(document.getElementById("num1").value);
			var num2 = parseInt(document.getElementById("num2").value);
			document.getElementById("result").value = num1 / num2;
		}
	</script>
</body>
</html>
