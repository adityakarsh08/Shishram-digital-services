<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Shishram Digital Services</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      background: #f4f6f8;
      color: #222;
      line-height: 1.6;
    }

    header {
      background: #111827;
      color: white;
      text-align: center;
      padding: 35px 15px;
    }

    header h1 {
      font-size: 30px;
      margin-bottom: 8px;
    }

    header p {
      font-size: 16px;
    }

    nav {
      background: white;
      padding: 12px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 10;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
    }

    nav a {
      color: #111827;
      text-decoration: none;
      margin: 0 8px;
      font-weight: bold;
      font-size: 14px;
    }

    .container {
      width: 100%;
      max-width: 950px;
      margin: auto;
      padding: 20px 15px;
    }

    section {
      background: white;
      padding: 25px 18px;
      margin: 20px 0;
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.07);
    }

    section h2 {
      color: #111827;
      margin-bottom: 15px;
      text-align: center;
    }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
    }

    .service {
      background: #f8fafc;
      border: 1px solid #e5e7eb;
      padding: 20px;
      border-radius: 12px;
      text-align: center;
    }

    .service h3 {
      margin-bottom: 8px;
    }

    .contact-box {
      text-align: center;
    }

    .number {
      font-size: 22px;
      font-weight: bold;
      margin: 15px 0;
      word-break: break-word;
    }

    .btn {
      display: inline-block;
      padding: 12px 18px;
      margin: 6px 3px;
      border-radius: 8px;
      text-decoration: none;
      color: white;
      font-weight: bold;
      border: none;
      cursor: pointer;
      font-size: 15px;
    }

    .call {
      background: #2563eb;
    }

    .whatsapp {
      background: #16a34a;
    }

    .copy {
      background: #4b5563;
    }

    footer {
      background: #111827;
      color: white;
      text-align: center;
      padding: 25px 15px;
      margin-top: 30px;
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 25px;
      }

      nav a {
        display: inline-block;
        margin: 4px;
      }

      section {
        padding: 22px 14px;
      }
    }
  </style>
</head>

<body>

  <header>
    <h1>Shishram Digital Services</h1>
    <p>आपकी डिजिटल सेवाओं का आसान समाधान</p>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#charges">Charges</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <main class="container">

    <section id="home">
      <h2>Welcome</h2>
      <p style="text-align:center;">
        Shishram Digital Services में आपका स्वागत है।
        हमारी डिजिटल सेवाओं की जानकारी नीचे दी गई है।
      </p>
    </section>

    <section id="services">
      <h2>Digital Services</h2>

      <div class="services">

        <div class="service">
          <h3>📝 Online Forms</h3>
          <p>Online form भरने में सहायता।</p>
        </div>

        <div class="service">
          <h3>📄 Documents</h3>
          <p>Document और PDF से जुड़ी डिजिटल सेवाएँ।</p>
        </div>

        <div class="service">
          <h3>🖨️ Print & Scan</h3>
          <p>Print, scan और document services।</p>
        </div>

        <div class="service">
          <h3>🎓 Education</h3>
          <p>Online registration और application assistance।</p>
        </div>

        <div class="service">
          <h3>🏛️ Application Help</h3>
          <p>Online applications में सहायता।</p>
        </div>

        <div class="service">
          <h3>💻 Digital Work</h3>
          <p>अन्य सामान्य digital services।</p>
        </div>

      </div>
    </section>

    <section id="charges">
      <h2>Service Charges</h2>

      <p style="text-align:center;">
        अलग-अलग सेवाओं की फीस सेवा के अनुसार तय की जाती है।
        फीस की जानकारी के लिए संपर्क करें।
      </p>
    </section>

    <section id="about">
      <h2>About Us</h2>

      <p style="text-align:center;">
        Shishram Digital Services एक digital service platform है,
        जहाँ ग्राहकों को विभिन्न online और digital कामों में सहायता दी जाती है।
      </p>
    </section>

    <section id="contact">
      <h2>Contact Us</h2>

      <div class="contact-box">

        <!-- यहाँ अपना नंबर डालें -->
        <div class="number" id="phoneNumber">YOUR_NUMBER</div>

        <button class="btn copy" onclick="copyNumber()">
          📋 Copy Number
        </button>

        <!-- YOUR_NUMBER को अपने नंबर से बदलें -->
        <a class="btn call" href="tel:YOUR_NUMBER">
          📞 Call Now
        </a>

        <!-- 91 के बाद अपना WhatsApp नंबर डालें -->
        <a class="btn whatsapp" href="https://wa.me/91YOUR_NUMBER">
          💬 WhatsApp
        </a>

      </div>
    </section>

  </main>

  <footer>
    © 2026 Shishram Digital Services
  </footer>

  <script>
    function copyNumber() {
      const number = document.getElementById("phoneNumber").innerText;

      navigator.clipboard.writeText(number);

      alert("Mobile number copied!");
    }
  </script>

</body>
</html>
