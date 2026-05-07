HTML<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Positioning Playground</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- HEADER FIXED -->
  <header class="header">
    <div class="logo">MyLogo</div>
    <nav class="nav">
      <a href="#">Home</a>
      <a href="#">Products</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- MAIN LAYOUT -->
  <div class="container">

    <!-- SIDEBAR STICKY -->
    <aside class="sidebar">
      <h3>Sidebar</h3>
      <p>Menu item 1</p>
      <p>Menu item 2</p>
      <p>Menu item 3</p>
      <p>Menu item 4</p>
    </aside>

    <!-- CONTENT -->
    <main class="content">

      <h2>Product List</h2>

      <!-- PRODUCT CARD -->
      <div class="card">
        <div class="badge">HOT</div>
        <h3>Product 1</h3>
        <p>Mô tả sản phẩm...</p>
      </div>

      <div class="card">
        <div class="badge">HOT</div>
        <h3>Product 2</h3>
        <p>Mô tả sản phẩm...</p>
      </div>

      <div class="card">
        <div class="badge">HOT</div>
        <h3>Product 3</h3>
        <p>Mô tả sản phẩm...</p>
      </div>

      <p style="height: 1000px;"></p> <!-- tạo scroll -->

    </main>
  </div>

  <!-- SCROLL TO TOP BUTTON -->
  <button class="to-top">↑</button>

</body>
</html>





CSS:


/* RESET */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* HEADER FIXED */
.header {
  position: fixed;
  top: 0;
  left: 0;
  height: 60px;
  width: 100%;
  background: #222;
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
  z-index: 1000;
}

.nav a {
  color: white;
  margin-left: 15px;
  text-decoration: none;
}

/* LAYOUT */
.container {
  display: flex;
  margin-top: 60px; /* tránh header che */
}

/* SIDEBAR STICKY */
.sidebar {
  width: 250px;
  padding: 20px;
  background: #f2f2f2;
  position: sticky;
  top: 80px; /* dưới header */
  height: fit-content;
}

/* CONTENT */
.content {
  flex: 1;
  padding: 20px;
}

/* PRODUCT CARD */
.card {
  width: 300px;
  padding: 20px;
  margin-bottom: 20px;
  border: 1px solid #ccc;
  position: relative;
  background: white;
}

/* HOT BADGE */
.badge {
  position: absolute;
  top: 10px;
  right: 10px;
  background: red;
  color: white;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 12px;
  font-weight: bold;
}

/* SCROLL TO TOP BUTTON */
.to-top {
  position: fixed;
  bottom: 20px;
  right: 20px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  border: none;
  background: #222;
  color: white;
  font-size: 20px;
  cursor: pointer;
}

<img width="1919" height="621" alt="image" src="https://github.com/user-attachments/assets/10c39085-b8bf-4142-8007-a06734956450" />

