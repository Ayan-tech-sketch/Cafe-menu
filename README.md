# Cafe-menu
<!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cafe Menu</title>
<style>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background: #f8f5f2;
}
header {
    background: #6b3e26;
    color: white;
    text-align: center;
    padding: 20px;
}
.container {
    padding: 20px;
}
.menu-item {
    background: white;
    margin: 10px 0;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
button {
    background: #6b3e26;
    color: white;
    border: none;
    padding: 10px 15px;
    border-radius: 5px;
    cursor: pointer;
}
input {
    padding: 10px;
    width: 70%;
    margin-right: 10px;
}
#viewer {
    margin-top: 20px;
    width: 100%;
    height: 400px;
    border: none;
    border-radius: 10px;
}
</style>
</head>
<body><header>
    <h1>My Cafe Menu</h1>
    <p>Explore our menu & 360° Cafe View</p>
</header><div class="container">
    <h2>Menu</h2><div class="menu-item">☕ Cappuccino - ₹120</div>
<div class="menu-item">🍕 Margherita Pizza - ₹250</div>
<div class="menu-item">🥪 Sandwich - ₹150</div>
<div class="menu-item">🍰 Chocolate Cake - ₹180</div>

<h2>Enter 360° View Link</h2>
<input type="text" id="linkInput" placeholder="Paste your 360° view link here">
<button onclick="loadView()">View Cafe</button>

<iframe id="viewer"></iframe>

</div><script>
function loadView() {
    let link = document.getElementById("linkInput").value;
    document.getElementById("viewer").src = link;
}
</script></body>
</html>
