# love
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Envelope Interaction</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        #envelope {
            width: 200px;
            height: 150px;
            background-color: #f0e68c;
            border: 2px solid #d1b000;
            position: relative;
            cursor: pointer;
            margin: auto;
        }
        #content {
            display: none;
            margin-top: 20px;
            font-size: 18px;
        }
        #finalMessage {
            display: none;
            margin-top: 20px;
            font-size: 20px;
            color: #ff69b4;
        }
    </style>
</head>
<body>

    <div id="envelope" onclick="openEnvelope()">
        Click to Open Envelope
    </div>
    
    <div id="content">
        Start na us sa isang stage, next naman na page "I know di mo magets HAHAHA, ang ibig kong sabihin ay........."
        <br>
        <button onclick="showFinalMessage()">Next</button>
    </div>
    
    <div id="finalMessage">
        I hope na gets muna, so yess I'll be your official girlfriend, babygurl, abby.
    </div>

    <script>
        function openEnvelope() {
            document.getElementById('content').style.display = 'block';
            document.getElementById('envelope').style.display = 'none';
        }

        function showFinalMessage() {
            document.getElementById('finalMessage').style.display = 'block';
            document.getElementById('content').style.display = 'none';
        }
    </script>

</body>
</html>
