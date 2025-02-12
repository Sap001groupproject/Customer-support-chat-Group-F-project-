# Customer-support-chat-Group-F-project-
<!DOCTYPE html>
<html>
<head>
  <title>Customer Attending Chat Support</title>
  <link rel="stylesheet" href="style.css">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Customer attending chat support website">
  <meta name="keywords" content="customer support, chat support, attending chat">
  <script type="text/javascript">
    var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();
    (function(){
      var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
      s1.async=true;
      s1.src='https://embed.tawk.to/your-widget-id/your-widget-name';
      s1.charset='UTF-8';
      s1.setAttribute('crossorigin','*');
      s0.parentNode.insertBefore(s1,s0);
    })();
  </script>
</head>
<body>
  <!-- Header Section -->
  <header>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About Us</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
    </nav>
  </header>
  <!-- Hero Section -->
  <section class="hero">
    <h1>Customer Attending Chat Support</h1>
    <p>We're here to help you with any questions you may have.</p>
    <button id="start-chat-button">Start Chat</button>
    <div>
      <a href="#" onclick="Tawk_API.toggle()">Chat with us</a>
    </div>
  </section>
  <!-- Chat Container -->
  <div class="chat-container">
    <div class="chat-header">
      <h2>Customer Attending Chat Support</h2>
      <span id="timestamp"></span>
    </div>
    <div class="customer-info">
      <input type="text" id="customer-name" placeholder="Your Name">
      <input type="email" id="customer-email" placeholder="Your Email">
    </div>
    <div class="chat-messages" id="chat-messages"></div>
    <div class="chat-input">
      <input type="text" id="message-input" placeholder="How May I Help You...">
      <button id="send-button">Send</button>
      <button id="attach-file-button">Attach File</button>
    </div>
    <div class="support-agent-info">
      <span id="support-agent-name"></span>
      <img id="support-agent-profile-picture" src="profile-picture.jpg">
    </div>
  </div>
  <!-- Footer Section -->
  <footer>
    <p>&copy;SAP001 2024 Customer Attending Chat Support</p>
    <ul>
      <li><a href="#">Terms and Conditions</a></li>
      <li><a href="#">Privacy Policy</a></li>
    </ul>
  </footer>
  <script src="script.js"></script>
</body>
</html>
