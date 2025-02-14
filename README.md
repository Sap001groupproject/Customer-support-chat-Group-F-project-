<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Customer Attending Chat Support</title>
  <meta name="description" content="Customer attending chat support website">
  <meta name="keywords" content="customer support, chat support, attending chat">
  <meta name="author" content="Your Company Name">
  <meta name="robots" content="index, follow">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    /* General Styles */
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      color: white;
      line-height: 1.6;
    }

    html {
      scroll-behavior: smooth;
    }

    /* Header Styles */
    header {
      background: rgba(0, 0, 0, 0.5);
      padding: 20px 0;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      backdrop-filter: blur(10px);
    }

    header nav ul {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
      justify-content: center;
      gap: 30px;
    }

    header nav ul li {
      display: inline;
    }

    header nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      font-size: 1.1rem;
      transition: color 0.3s ease;
    }

    header nav ul li a:hover {
      color: #ff6f61;
    }

    /* Hero Section Styles */
    .hero {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      background: url('https://via.placeholder.com/1200x800') no-repeat center center/cover;
      position: relative;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.5);
    }

    .hero h1 {
      font-size: 3.5rem;
      margin-bottom: 10px;
      z-index: 1;
      animation: fadeIn 2s ease-in-out;
    }

    .hero p {
      font-size: 1.5rem;
      margin-bottom: 30px;
      z-index: 1;
      animation: fadeIn 2.5s ease-in-out;
    }

    .hero button {
      background: #ff6f61;
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 1.2rem;
      cursor: pointer;
      border-radius: 50px;
      transition: background 0.3s ease, transform 0.3s ease;
      z-index: 1;
    }

    .hero button:hover {
      background: #ff4a3d;
      transform: scale(1.1);
    }

    /* Footer Styles */
    footer {
      background: rgba(0, 0, 0, 0.7);
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
      backdrop-filter: blur(10px);
    }

    footer ul {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
      justify-content: center;
      gap: 20px;
    }

    footer ul li {
      display: inline;
    }

    footer ul li a {
      color: white;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    footer ul li a:hover {
      color: #ff6f61;
    }

    /* Animations */
    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2.5rem;
      }

      .hero p {
        font-size: 1.2rem;
      }

      header nav ul {
        flex-direction: column;
        gap: 10px;
      }

      footer ul {
        flex-direction: column;
        gap: 10px;
      }
    }
  </style>
</head>
<body>
  <!-- Header Section -->
  <header>
    <nav>
      <ul>
        <li><a href="#" aria-label="Home">Home</a></li>
        <li><a href="#" aria-label="About Us">About Us</a></li>
        <li><a href="#" aria-label="Contact Us">Contact Us</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Customer Attending Chat Support</h1>
    <p>We're here to help you with any questions you may have.</p>
    <button id="start-chat-button" aria-label="Start Chat">Start Chat</button>
  </section>

  <!-- Footer Section -->
  <footer>
    <p>&copy; SAP001 2024 Customer Attending Chat Support</p>
    <ul>
      <li><a href="#" aria-label="Terms and Conditions">Terms and Conditions</a></li>
      <li><a href="#" aria-label="Privacy Policy">Privacy Policy</a></li>
    </ul>
  </footer>

  <!-- IBM Watson Assistant Chat Integration -->
  <script>
    window.watsonAssistantChatOptions = {
      integrationID: "37414c5c-8d93-4252-a773-eaddeae6ae28", // Replace with your integration ID
      region: "us-south", // Replace with your region
      serviceInstanceID: "a59cb452-2d24-46a7-9f10-69ced278a669", // Replace with your service instance ID
      onLoad: function(instance) {
        instance.render();
      }
    };

    setTimeout(function() {
      const t = document.createElement('script');
      t.src = "https://web-chat.global.assistant.watson.appdomain.cloud/versions/" + (window.watsonAssistantChatOptions.clientVersion || 'latest') + "/WatsonAssistantChatEntry.js";
      document.head.appendChild(t);
    });

    // Toggle chat on button click
    document.getElementById('start-chat-button').addEventListener('click', function() {
      window.watsonAssistantChatInstance.toggleOpen();
    });
  </script>
</body>
</html>