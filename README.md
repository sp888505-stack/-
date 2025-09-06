<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>普洱茶銷售網站</title>
  <style>
    body {
      margin: 0;
      font-family: "Microsoft JhengHei", sans-serif;
      line-height: 1.6;
      background-color: #fdfcf7;
      color: #333;
    }
    header {
      background: #3e2723;
      color: #fff;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    header h1 { margin: 0; font-size: 22px; }
    nav a {
      color: #fff;
      text-decoration: none;
      margin: 0 12px;
      font-weight: bold;
    }
    nav a:hover { color: #ffc107; }

    .banner {
      background: url("https://images.unsplash.com/photo-1583224083224-4b9fbf4e8ebf") center/cover no-repeat;
      color: white;
      height: 350px;
      display: flex;
      justify-content: center;
      align-items: center;
      text-shadow: 2px 2px 5px rgba(0,0,0,0.7);
    }
    .banner h2 {
      font-size: 40px;
      background: rgba(0,0,0,0.4);
      padding: 10px 20px;
      border-radius: 10px;
    }

    section { padding: 60px 20px; max-width: 1100px; margin: auto; }
    section h2 { text-align: center; margin-bottom: 30px; }

    /* 商品展示 */
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .product {
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      overflow: hidden;
      text-align: center;
      transition: transform 0.2s;
    }
    .product:hover { transform: scale(1.03); }
    .product img { width: 100%; height: 200px; object-fit: cover; }
    .product h3 { margin: 15px 0 5px; }
    .product p { margin: 5px 0; }
    .btn {
      display: inline-block;
      margin: 10px 0 20px;
      padding: 8px 16px;
      background: #3e2723;
      color: #fff;
      border-radius: 5px;
      text-decoration: none;
    }
    .btn:hover { background: #5d4037; }

    /* 聯絡表單 */
    form {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-direction: column;
    }
    form input, form textarea {
      margin-bottom: 15px;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 16px;
    }
    form button {
      padding: 10px;
      background: #3e2723;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    form button:hover { background: #5d4037; }

    footer {
      background: #3e2723;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <header>
    <h1>普洱茶坊</h1>
    <nav>
      <a href="#home">首頁</a>
      <a href="#products">商品</a>
      <a href="#contact">聯絡我們</a>
    </nav>
  </header>

  <section id="home" class="banner">
    <h2>品味雋永的普洱茶</h2>
  </section>

  <section id="intro">
    <h2>關於我們</h2>
    <p style="text-align:center;">
      我們專注於嚴選上等普洱茶，讓每一位茶友都能品嚐到純正、健康與自然的風味。  
      無論是生茶的清新，還是熟茶的醇厚，這裡都有最適合你的選擇。
    </p>
  </section>

  <section id="products">
    <h2>熱銷商品</h2>
    <div class="products">
      <div class="product">
        <img src="https://images.unsplash.com/photo-1584380931060-1c54f2f04f66" alt="普洱生茶">
        <h3>普洱生茶</h3>
        <p>NT$ 1200</p>
        <a href="#" class="btn">加入購物車</a>
      </div>
      <div class="product">
        <img src="https://images.unsplash.com/photo-1582531799725-86dba7d62a9e" alt="普洱熟茶">
        <h3>普洱熟茶</h3>
        <p>NT$ 1500</p>
        <a href="#" class="btn">加入購物車</a>
      </div>
      <div class="product">
        <img src="https://images.unsplash.com/photo-1607956352632-75b8f4f26d09" alt="古樹普洱">
        <h3>古樹普洱</h3>
        <p>NT$ 2500</p>
        <a href="#" class="btn">加入購物車</a>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>聯絡我們</h2>
    <form>
      <input type="text" placeholder="姓名" required>
      <input type="email" placeholder="Email" required>
      <textarea rows="5" placeholder="留言內容" required></textarea>
      <button type="submit">送出</button>
    </form>
  </section>

  <footer>
    <p>© 2025 普洱茶坊 | 版權所有</p>
  </footer>
</body>
</html>
