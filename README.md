<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>كلمة المرور</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }
        #message {
            display: none;
            color: green;
            font-size: 24px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div>
        <label for="password">أدخل كلمة المرور:</label>
        <input type="password" id="password">
        <button onclick="checkPassword()">تأكيد</button>
        <p id="message">تزعل الدنيا كلها ولا تزعل حوريتي الحلوة</p>
    </div>

    <script>
        function checkPassword() {
            const password = document.getElementById('password').value;
            const message = document.getElementById('message');
            const correctPassword = "حوريتي الحلوة"; // كلمة المرور

            if (password === correctPassword) {
                message.style.display = 'block';
            } else {
                message.style.display = 'none';
                alert('كلمة المرور غير صحيحة');
            }
        }
    </script>
</body>
</html>
