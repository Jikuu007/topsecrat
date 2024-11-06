<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lier_Web</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            text-align: center ;
            background-color: #333;
            color: #fff;
        }
        h1 {
            color: #ff3333;
        }
        .button {
            margin: 10px;
            padding:  10px 20px;
            font-size: 18px;
            color: #fff;
            background-color: #555;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .button:hover {
            background-color: #f33;
        }
    </style>
</head>
<body>
    <h1>Funny</h1>
    <p>Sélectionnez le son que vous souhaitez utiliser pour faire une farce à votre ami!</p>
    
    <button class = "button" onclick="playsound('scream')">Criant</button>
    <audio id="scream" src="scream.mp3"></audio>
    <script>
        function playsound(id){
            const sound = document.getElementById(id);
            sound.currentTime = 0;
            sound.play();
        }
    </script>
</body>
</html>