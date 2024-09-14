<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leap Year Checker</title>
    <script>
        function checkLeapYear() {
            var year = parseInt(document.getElementById('year').value);
            var result = document.getElementById('result');
            
            if ((year % 4 === 0 && year % 100 !== 0) || (year % 400 === 0)) {
                result.textContent = year + " is a leap year.";
            } else {
                result.textContent = year + " is not a leap year.";
            }
        }
    </script>
</head>
<body>
    <h1>Leap Year Checker</h1>
    <input type="number" id="year" placeholder="Enter a year" />
    <button onclick="checkLeapYear()">Check</button>
    <p id="result"></p>
</body>
</html>
