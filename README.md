#<!DOCTYPE html>
#<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Gradient Table</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #0033cc 0%, #00de94 100%);
            animation: gradient 15s ease infinite;  
            background-size: 400% 400%;
        }

        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        table {
            border-collapse: separate;
            border-spacing: 20px; /* Adds a gap between rows and columns */
            width: 60%;
            max-width: 600px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        th, td {
            padding: 20px;
            text-align: center;
            border: 1px solid #ddd;
            background: rgba(255, 255, 255, 0.8);
            transition: transform 0.2s;
        }

        th:hover, td:hover {
            transform: scale(1.1);
            background: rgba(255, 255, 255, 1);
        }

        th {
            background: rgba(255, 255, 255, 0.9);
        }
        a{
            text-decoration: none;
        }
    </style>
</head>
<body>
    <table>
        <tr>
            <th>PHP</th>
            <th>JAVA</th>
        </tr>
        <tr>
            <td>Cell 1</td>
            <td>Cell 2</td>
        </tr>
        <tr>
            <td>Cell 3</td>
            <td>Cell 4</td>
        </tr>
    </table>
</body>
</html>
