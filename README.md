<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Seanampal ka ba?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            color: #333;
            text-align: center;
        }

        header {
            background-color: #034EA2;
            color: white;
            padding: 10px;
        }

        nav a {
            text-decoration: none;
            color: #333;
            padding: 10px;
        }

        section {
            margin: 20px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            justify-items: center;
        }

        .menu-item {
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 10px;
            background-color: white;
        }

        footer {
            background-color: #034EA2;
            color: white;
            padding: 10px;
        }
    </style>
</head>

<body>
    <header>
                <img src="C:\Users\User\Downloads\images1\436210379_2254203008272859_3903604409828590263_n.jpg" alt="sinampal">
        <h1>Seanampal  </h1>
        <p>Best in Filipino Cuisine na sinasampal!</p>
    </header>

    <nav>
        <a href="#">Home</a>
        <a href="#">Menu</a>
        <a href="#">Contact</a>
    </nav>

    <section>
        <h2>Menu</h2>
        <div class="grid">
            <div class="menu-item">
                <img src="C:\Users\User\Downloads\images1\Beef-Pares-Recipe.jpg" alt="Pares">
                <h3>Diwata Pares</h3>
                <p>Price: PHP 100</p>
                <button onclick="orderItem(100)">Order</button>
            </div>

            <div class="menu-item">
                <img src="C:\Users\User\Downloads\images1\OIP.jpg" alt="Adobo">
                <h3>Adobo</h3>
                <p>Price: PHP 150</p>
                <button onclick="orderItem(150)">Order</button>
            </div>

            <!-- Add more menu items here -->
        </div>

        <h3>Total: PHP <span id="total">0.00</span></h3>
    </section>

    <footer>
        <p>&copy; 2024 Seanampal | Designed by Sean Arlhon Roxas, Lleyton Cleodoro, Jan Mateo Tibon, and Elijah Reyn</p>
    </footer>

    <script>
        let total = 0;

        function orderItem(price) {
            total += price;
            document.getElementById('total').textContent = total.toFixed(2);
        }
    </script>
</body>

</html>
