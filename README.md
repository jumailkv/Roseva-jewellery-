
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ROSÉVA | Jewellery</title>
<style>
:root{--green:#526653;--cream:#f8f5ef;--ink:#252920}
*{box-sizing:border-box}
body{margin:0;background:var(--cream);color:var(--ink);font-family:Arial,sans-serif}
header{padding:22px 18px;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid #deded3}
.logo{font-family:Georgia,serif;font-size:28px;letter-spacing:4px;color:var(--green)}
header a{color:var(--green);text-decoration:none;font-size:13px}
.hero{text-align:center;padding:62px 20px 48px}
.hero small{letter-spacing:3px;color:var(--green)}
h1{font:normal 42px Georgia,serif;line-height:1.15;margin:18px 0}
.hero p{color:#696b60;line-height:1.7;font-size:14px}
.btn{display:inline-block;background:var(--green);color:white;padding:14px 24px;text-decoration:none;margin-top:14px;font-size:13px;letter-spacing:1px}
section{padding:20px 18px 45px}
.section-title{text-align:center;font:normal 29px Georgia,serif;margin:10px 0}
.sub{text-align:center;color:#777;font-size:13px;margin-bottom:28px}
.products{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.product{background:#fff;padding-bottom:16px}
.product-art{height:165px;background:#e9e4d9;display:flex;align-items:center;justify-content:center;font-size:66px}
.product h3{font:normal 17px Georgia,serif;margin:13px 10px 6px}
.price{margin:0 10px 12px;color:var(--green);font-size:14px}
.order{display:block;text-align:center;margin:0 10px;padding:11px 5px;border:1px solid var(--green);color:var(--green);text-decoration:none;font-size:12px}
.note{text-align:center;padding:30px 20px;background:#eeeadf;font:normal 23px Georgia,serif;line-height:1.5}
footer{text-align:center;padding:25px 10px;color:#686b60;font-size:12px}
</style>
</head>
<body>
<header>
  <div class="logo">ROSÉVA</div>
  <a href="#collection">OUR COLLECTION ↓</a>
</header>
<div class="hero">
  <small>EVERYDAY ELEGANCE</small>
  <h1>Jewellery that<br>feels like you.</h1>
  <p>Discover timeless pieces made to<br>make your everyday moments special.</p>
  <a class="btn" href="#collection">EXPLORE COLLECTION</a>
</div>
<section id="collection">
  <h2 class="section-title">The Collection</h2>
  <p class="sub">Simple pieces. Lasting impressions.</p>
  <div class="products">
    <article class="product">
      <div class="product-art">♡</div>
      <h3>Everyday Chain</h3>
      <p class="price">₹499</p>
      <a class="order" href="#" onclick="order('Everyday Chain',499);return false">ORDER ON WHATSAPP</a>
    </article>
    <article class="product">
      <div class="product-art">✧</div>
      <h3>Golden Layer Chain</h3>
      <p class="price">₹599</p>
      <a class="order" href="#" onclick="order('Golden Layer Chain',599);return false">ORDER ON WHATSAPP</a>
    </article>
    <article class="product">
      <div class="product-art">◇</div>
      <h3>Minimal Pendant</h3>
      <p class="price">₹449</p>
      <a class="order" href="#" onclick="order('Minimal Pendant',449);return false">ORDER ON WHATSAPP</a>
    </article>
    <article class="product">
      <div class="product-art">∞</div>
      <h3>Classic Chain</h3>
      <p class="price">₹699</p>
      <a class="order" href="#" onclick="order('Classic Chain',699);return false">ORDER ON WHATSAPP</a>
    </article>
  </div>
</section>
<div class="note">“A little elegance,<br>every single day.”</div>
<footer>ROSÉVA · JEWELLERY<br><br>For orders and enquiries, contact us on WhatsApp.</footer>
<script>
function order(name,price){
  const phone="91XXXXXXXXXX";
  if(phone.includes("X")){
    alert("WhatsApp number setup is needed before ordering. Please contact ROSÉVA directly.");
    return;
  }
  const msg=encodeURIComponent("Hello ROSÉVA! I would like to order "+name+" for ₹"+price+".");
  window.open("https://wa.me/"+phone+"?text="+msg,"_blank");
}
</script>
</body>
</html>
