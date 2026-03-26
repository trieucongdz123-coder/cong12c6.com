# cong12c6.com
Tuyên Quang
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KOREAN MEN STYLE 2026</title>

<style>
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: #f8f8f8;
}

/* HEADER */
header {
    background: white;
    padding: 15px 30px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0 2px 5px rgba(0,0,0,0.05);
}

.logo {
    font-weight: bold;
    font-size: 22px;
}

nav a {
    margin: 0 15px;
    text-decoration: none;
    color: black;
}

/* BANNER */
.banner {
    background: url('https://i.imgur.com/8Km9tLL.jpg') center/cover;
    height: 400px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-size: 32px;
    font-weight: bold;
}

/* SECTION */
.container {
    padding: 40px;
}

h2 {
    text-align: center;
    margin-bottom: 30px;
}

/* PRODUCT GRID */
.products {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 20px;
}

.card {
    background: white;
    padding: 15px;
    border-radius: 10px;
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-5px);
}

.card img {
    width: 100%;
    border-radius: 10px;
}

.card h3 {
    margin: 10px 0 5px;
}

.price {
    color: #e60023;
    font-weight: bold;
}

button {
    width: 100%;
    padding: 10px;
    border: none;
    background: black;
    color: white;
    cursor: pointer;
    margin-top: 10px;
}

/* CART */
.cart {
    position: fixed;
    top: 20px;
    right: 20px;
    background: white;
    padding: 15px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 0 10px rgba(0,0,0,0.2);
}

footer {
    text-align: center;
    padding: 20px;
    background: black;
    color: white;
    margin-top: 40px;
}
</style>
</head>

<body>

<header>
    <div class="logo">K-STYLE 2026</div>
    <nav>
        <a href="#">Trang chủ</a>
        <a href="#">Sản phẩm</a>
        <a href="#">Xu hướng</a>
        <a href="#">Liên hệ</a>
    </nav>
</header>

<div class="banner">
    Korean Style - Chuẩn Gu Gen Z
</div>

<div class="container">
    <h2>Sản phẩm nổi bật</h2>

    <div class="products">

        <div class="card">
            <img src="https://i.imgur.com/ZF6s192.jpg">
            <h3>Áo thun oversize</h3>
            <p class="price">199.000đ</p>
            <button onclick="addToCart('Áo thun oversize',199000)">Mua</button>
        </div>

        <div class="card">
            <img src="https://i.imgur.com/1ZQZ1Zm.jpg">
            <h3>Quần ống rộng</h3>
            <p class="price">299.000đ</p>
            <button onclick="addToCart('Quần ống rộng',299000)">Mua</button>
        </div>

        <div class="card">
            <img src="https://i.imgur.com/3ZQ3ZQx.jpg">
            <h3>Áo sơ mi Hàn</h3>
            <p class="price">249.000đ</p>
            <button onclick="addToCart('Áo sơ mi Hàn',249000)">Mua</button>
        </div>

        <div class="card">
            <img src="https://i.imgur.com/YW6Fufc.jpg">
            <h3>Set outfit full</h3>
            <p class="price">499.000đ</p>
            <button onclick="addToCart('Set outfit',499000)">Mua</button>
        </div>

    </div>
</div>

<div class="container">
    <h2>Xu hướng 2026</h2>
    <p style="text-align:center;">
        Phong cách Hàn Quốc tối giản, form rộng, màu trung tính đang dẫn đầu xu hướng.
    </p>
</div>

<div class="container">
    <h2>Liên hệ</h2>
    <p style="text-align:center;">Zalo: 0123456789 | Facebook: yourlink</p>
</div>

<!-- CART -->
<div class="cart">
    <h3>🛒 Giỏ hàng</h3>
    <ul id="cart-list"></ul>
    <p><b>Tổng: <span id="total">0</span>đ</b></p>
</div>

<footer>
    © 2026 K-STYLE
</footer>

<script>
let total = 0;

function addToCart(name, price) {
    let li = document.createElement("li");
    li.textContent = name + " - " + price + "đ";
    document.getElementById("cart-list").appendChild(li);

    total += price;
    document.getElementById("total").innerText = total;
}
</script>

</body>
</html>
