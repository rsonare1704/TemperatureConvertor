# TemperatureConvertor
First task given by Bharat Intern



<!DOCTYPE html>
<html>
<head>
  <title>Temperature Converter</title>
  <style>
  body {
    font-family: Arial, sans-serif;
    background-color:lightgrey;
    margin-top: 150px;
    bor
  }
  
  h1 {
    text-align: center;
    color: darkcyan;
    margin-top: 150px;

  }
  
  .container {
    margin: 30px;
  }
  
  label {
    display: block;
    margin-bottom: 5px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }
  
  input {
    padding: 7px;
    width: 200px;
    text-decoration:solid;
  }
  
  button {
    padding: 10px 20px;
    background-color: rgb(68, 8, 142);
    color: white;
    border:darkkhaki;
    cursor: pointer;
  }
  
  .result-container {
    margin: 30px;
    background-color: rgb(161, 156, 158);
    padding: 10px;
  }
  
  #result {
    font-size: 18px;
    font-weight:lighter;
    text-decoration: underline;
    color: rgb(12, 6, 7);
    text-decoration: solid;
  }
  h6{
    text-align: center;
  }
 body hr{
    border:0px;
    background-color: black;
    height: 2px;
    margin: 60px 84px;
  }
  </style>
  
</head>
<body>
  <i><h1>Temperature Converter</h1></i>
  <hr>

  <div class="container">
    <label for="celsius"><u>Celsius:</label></u>
    <input type="number" id="celsius" placeholder="Enter temperature in Celsius">
    <button id="convertBtn" onclick="convertTemperature()">Convert</button>
  </div>

  <div class="result-container">
    <h3>Result:</h3>
    <div id="result"></div>
  </div>
  <hr>

  <script>
  function convertTemperature() {
    var celsiusInput = document.getElementById("celsius");
    var celsius = parseFloat(celsiusInput.value);
  
    if (!isNaN(celsius)) {
      var fahrenheit = (celsius * 9/5) + 32;
      var resultElement = document.getElementById("result");
      resultElement.innerHTML = celsius + "°C is equal to " + fahrenheit.toFixed(2) + "°F";
    }
  }
</script>
<br><br><br><br><br><br><br>

<u><i><h6>Project:Temperature Converter</h6></i></u>
<u><i><h6>By:Rohit Sonare</h6></i></u>

</body>
</html>
