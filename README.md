<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thông tin tiểu sử và khảo sát</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        #container {
            max-width: 800px;
            margin: 20px auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1, h2 {
            text-align: center;
        }

        form {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 5px;
        }

        input[type="text"],
        input[type="date"] {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }

        button {
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }

        .question {
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <div id="container">
        <h1>Thông tin và khảo sát</h1>
        <div id="user-info">
            <h2>Nhập thông tin</h2>
            <form id="info-form">
                <label for="full-name">Họ và tên:</label>
                <input type="text" id="full-name" name="full-name" required><br>
                
                <label for="dob">Ngày tháng năm sinh:</label>
                <input type="date" id="dob" name="dob" required><br>
                
                <label for="cccd">CCCD:</label>
                <input type="text" id="cccd" name="cccd" required><br>
                
                <label for="address">Địa chỉ:</label>
                <input type="text" id="address" name="address" required><br>
                
                <button type="submit">Submit</button>
            </form>
        </div>
    </div>

    <script>
        document.getElementById('info-form').addEventListener('submit', function(event){
            event.preventDefault();

            window.location.href = 'exam.html';
        });
    </script>

</body>

</html>
