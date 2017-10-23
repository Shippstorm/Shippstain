# Shippstain
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="initial-scale=1, maximum-scale=1, user-scalable=no, width=device-width">
        <title>Dog Years Calculator</title>
        <link rel="stylesheet" href="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css" />
        <script src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
        <script src="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>
        <link rel="stylesheet" href="index2.css" type=text/css>
        <script>
        
        window.onload=function()
        {
            document.getElementById('btnCalc').addEventListener('click', calcAge);
        }
        
        function calcAge(e)
            {
                var age = document.getElementById('dogAge').value;
                age= age *7;
                var result = "In dog years, your dog is: " + age;
                console.log(result);
                document.getElementById('result').innerHTML = 
                result;
            }
        </script>
    </head>
    <body>
        <div data-role="page">
        <div data-role="header">
        <script type="text/javascript" src="cordova.js"></script>
        <h1>Dog years Calculator</h1>
        </div>
        <div data-role="main" class="ui-content">
        <label for="dogAge">Dog age in Human Years</label>
        <input id="dogAge" type="number" />
        <button id="btnCalc">Calculate</button>
        <div id="result"></div>
        </div>
        <div data-role="footer">
        <p>Snoop Doggy Dog</p>
        </div>
        </div>
    </body>
</html>
