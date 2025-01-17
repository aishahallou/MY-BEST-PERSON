# MY-BEST-PERSON
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Liebe Nachricht</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 50px;
        }
        h2 {
            color: #ff69b4;
        }
        .message {
            font-size: 20px;
            margin-top: 20px;
        }
        .heart {
            color: red;
        }
    </style>
</head>
<body>

    <h2>Gib deinen Namen ein</h2>
    <input type="text" id="nameInput" placeholder="Dein Name" />
    <button onclick="showMessage()">Absenden</button>

    <div id="message" class="message"></div>

    <script>
        function showMessage() {
            const name = document.getElementById('nameInput').value;
            if (name) {
                const message = `<p><span class="heart">💖</span> I love you, ${name} <span class="heart">💖</span></p>
                                <p>Knowing you feels like apricity on a freezing winter day!</p>
                                <p>You are such an incredible person, and you deserve all the best things life has to offer.</p>
                                <p>I believe in everything you do and know you’re capable of achieving amazing things.</p>
                                <p>I will always be here to support and cheer you!</p>
                                <p><strong>YOU DESERVE THE BEST, LOVE YOU SO MUCH!</strong></p>`;
                document.getElementById('message').innerHTML = message;
            } else {
                alert("Bitte gib deinen Namen ein!");
            }
        }
    </script>

</body>
</html>
