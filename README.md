<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Delicious Bites - Restaurant</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #fff8f0;
            color: #333;
        }
        a {
            text-decoration: none;
            color: inherit;
        }
        header {
            background: #d35400;
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        header h1 {
            font-size: 1.5rem;
        }
        nav ul {
            display: flex;
            list-style: none;
        }
        nav ul li {
            margin-left: 20px;
        }
        nav ul li a {
            font-weight: bold;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #ffeaa7;
        }
        .menu-toggle {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }
        @media (max-width: 768px) {
            nav ul {
                display: none;
                flex-direction: column;
                background: #d35400;
                position: absolute;
                top: 60px;
                right: 0;
                width: 200px;
                padding: 10px;
            }
            nav ul.show {
                display: flex;
            }
            .menu-toggle {
                display: block;
            }
        }
        .hero {
            background: url('https://images.unsplash.com/photo-1600891964599-f61ba0e24092') center/cover no-repeat;
            height: 60vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
        }
        .hero h2 {
            font-size: 2.5rem;
            background: rgba(0,0,0,0.5);
            padding: 10px 20px;
            border-radius: 5px;
        }
        .menu {
            padding: 40px 20px;
            max-width: 1000px;
            margin: auto;
        }
        .menu h2 {
            text-align: center;
            margin-bottom: 20px;
            color: #d35400;
        }
        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .menu-item {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        .menu-item:hover {
            transform: scale(1.05);
        }
        .menu-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        .menu-item h3 {
            padding: 10px;
            color: #d35400;
        }
        .menu-item p {
            padding: 0 10px 10px;
            font-size: 0.9rem;
        }

        footer {
            background: #d35400;
            color: white;
            text-align: center;
            padding: 15px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Delicious Bites</h1>
        <span class="menu-toggle" id="menu-toggle">&#9776;</span>
        <nav>
            <ul id="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <section class="hero" id="home">
        <h2>Welcome to Delicious Bites</h2>
    </section>
    <section class="menu" id="menu">
        <h2>Our Menu</h2>
        <div class="menu-items">
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1600891964599-f61ba0e24092" alt="Pizza">
                <h3>Margherita Pizza</h3>
                <p>Classic pizza with fresh mozzarella, tomatoes, and basil.</p>
            </div>
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1551218808-94e220e084d2" alt="Burger">
                <h3>Cheese Burger</h3>
                <p>Juicy beef patty with cheddar cheese, lettuce, and tomato.</p>
            </div>
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1546069901-ba9599a7e63c" alt="Pasta">
                <h3>Spaghetti Carbonara</h3>
                <p>Rich and creamy pasta with pancetta and parmesan.</p>
            </div>
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836" alt="Salad">
                <h3>Caesar Salad</h3>
                <p>Crisp romaine lettuce with Caesar dressing, croutons, and parmesan.</p>
        </div>
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1504754524776-8f4f37790ca0" alt="Sushi">
                <h3>Sushi Platter</h3>
                <p>Assorted fresh sushi rolls with wasabi and soy sauce.</p>
            </div>
            <div class="menu-item">
                <img src="OIP.jpg" alt="Dessert">
                <h3>Chocolate Lava Cake</h3>
                <p>Warm chocolate cake with a gooey molten center.</p>
        </div>
        <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1525755662778-989d0524087e" alt="Tacos">
                <h3>Fish Tacos</h3>
                <p>Grilled fish with fresh salsa and creamy sauce in soft tortillas.</p>
            </div>
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1490645935967-10de6ba17061" alt="Steak">
                <h3>Grilled Ribeye Steak</h3>
                <p>Juicy ribeye steak grilled to perfection, served with sides.</p>
        </div>
        <div class="menu-item">
                <img src="image.png" alt="Soup">
                <h3>Tomato Basil Soup</h3>
                <p>Rich and creamy tomato soup with fresh basil and a hint of garlic.</p>
        </div>
    <div>
        <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93" alt="Pancakes">
                <h3>Buttermilk Pancakes</h3>
                <p>Fluffy pancakes served with maple syrup and fresh berries.</p>
    </div>
        </div>    
    </section>
    <section class="menu" id="contact">
        <h2>Contact Us</h2>
        <p style="text-align:center;">📍 123 Food Street, My home Town<br>📞 +977 1234456700</p>
    </section>

    <footer>
        <p>&copy; 2026 Delicious Bites. All Rights Reserved.</p>
    </footer>
</body>
</html>
