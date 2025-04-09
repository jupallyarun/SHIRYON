<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>SHIRYON - Revolutionizing Your Gym Wardrobe</title>
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap"
      rel="stylesheet"
    />

    <style>
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

      body {
        font-family: 'Poppins', sans-serif;
        background-color: black; /* Black background */
        color: white; /* White text color */
        line-height: 1.6;
      }

      .site-header {
        padding: 50px 60px;
        color: white;
        text-align: left;
      }

      .site-title h1 {
        font-size: 60px; /* Increased font size */
        font-weight: 800; /* Made it bolder */
        margin-bottom: 10px;
        color: white;
      }

      .site-title p {
        font-size: 30px; /* Increased font size */
        font-weight: 800; /* Made it bolder */
        color: white;
        text-transform: uppercase;
        letter-spacing: 2px; /* Slightly increased letter-spacing */
      }

      .header-image-container {
        width: 100%;
        text-align: center;
        margin-top: 30px;
        background-color: black;
        padding: 20px;
      }

      .header-image {
        width: 100%;
        max-width: 600px; /* Restricts the width of the image */
        height: auto;
        object-fit: contain;
        border-radius: 8px;
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        animation: dynamicImageAnimation 10s infinite, logoShineEffect 2s infinite, logoMoveLeftRight 5s infinite alternate, rayOfLight 5s infinite;
      }

      /* Dynamic animation for the image (rotation, scale, and translate) */
      @keyframes dynamicImageAnimation {
        0% {
          transform: scale(1) rotate(0deg) translateX(0) translateY(0);
        }
        25% {
          transform: scale(1.1) rotate(5deg) translateX(10px) translateY(-10px);
        }
        50% {
          transform: scale(1.2) rotate(-5deg) translateX(-10px) translateY(10px);
        }
        75% {
          transform: scale(1.1) rotate(0deg) translateX(10px) translateY(-10px);
        }
        100% {
          transform: scale(1) rotate(0deg) translateX(0) translateY(0);
        }
      }

      /* Shine effect on the logo with a brighter, faster shine */
      @keyframes logoShineEffect {
        0% {
          filter: brightness(1);
        }
        50% {
          filter: brightness(2); /* Increased brightness */
        }
        100% {
          filter: brightness(1);
        }
      }

      /* Moving the logo from left to right with stronger movement */
      @keyframes logoMoveLeftRight {
        0% {
          transform: translateX(0);
        }
        50% {
          transform: translateX(50px); /* Increased movement */
        }
        100% {
          transform: translateX(0);
        }
      }

      /* Add a new 'Ray of Light' animation */
      @keyframes rayOfLight {
        0% {
          background: linear-gradient(to right, #ffffff, rgba(255, 255, 255, 0)); /* Create the ray effect */
        }
        100% {
          background: linear-gradient(to left, #ffffff, rgba(255, 255, 255, 0)); /* Full left-to-right shine */
        }
      }

      .section-wrapper {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 60px;
        padding: 70px 50px;
        max-width: 1200px;
        margin: auto;
      }

      .contact-box,
      .form-box {
        background: black;
        padding: 40px;
        border-radius: 15px;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        width: 100%;
        max-width: 500px;
      }

      .contact-box {
        flex: 1 1 300px;
      }

      .contact-box h3 {
        color: #007bff;
        margin-bottom: 20px;
        font-size: 28px;
      }

      .contact-box p {
        font-size: 18px;
        line-height: 1.8;
        margin-bottom: 20px;
      }

      .form-box {
        flex: 1 1 500px;
      }

      .form-box h2 {
        text-align: center;
        color: #007bff;
        margin-bottom: 30px;
        font-size: 30px;
      }

      form {
        display: flex;
        flex-direction: column;
        gap: 20px;
      }

      .name-fields {
        display: flex;
        gap: 20px;
      }

      .name-fields input {
        flex: 1;
        padding: 15px;
        border: 1px solid #ccc;
        border-radius: 10px;
        font-size: 18px;
      }

      input,
      textarea {
        padding: 15px;
        border: 1px solid #ccc;
        border-radius: 10px;
        font-size: 18px;
        background-color: #d3d3d3; /* Grey/Silver background for form fields */
        color: #333; /* Darker text color */
      }

      textarea {
        resize: vertical;
        min-height: 120px;
      }

      button {
        padding: 15px;
        background: linear-gradient(to right, #007bff, #00c6ff);
        color: white;
        border: none;
        border-radius: 10px;
        cursor: pointer;
        font-size: 18px;
        transition: background 0.3s;
      }

      button:hover {
        background: linear-gradient(to right, #0056b3, #0099cc);
      }

      footer {
        padding: 30px;
        background-color: transparent;
        color: white; /* White text for footer */
        font-size: 20px;
        font-weight: bold;
        text-align: left;
      }

      footer p {
        margin-bottom: 10px;
      }

      footer a {
        color: #f8fafa; /* Link color */
        text-decoration: none;
        font-weight: bold;
      }

      .Address {
        border-color: transparent;
      }

      @media (max-width: 768px) {
        .section-wrapper {
          flex-direction: column;
          padding: 50px 20px;
        }

        .name-fields {
          flex-direction: column;
        }

        .site-header {
          padding: 40px;
        }

        .site-title h1 {
          font-size: 40px;
        }

        .site-title p {
          font-size: 18px;
        }
      }
    </style>
  </head>
  <body>
    <div class="site-header">
      <div class="site-title">
        <h1>SHIRYON</h1>
        <p>Revolutionizing your gym wardrobe</p>
      </div>
    </div>

    <div class="header-image-container">
      <img
        class="header-image"
        src="https://i.postimg.cc/GmYmt6gW/IMG-4601.png"
        alt="Gym Fashion"
      />
    </div>

    <div class="section-wrapper">
      <div class="contact-box">
        <h3>Contact Us</h3>
        <p>Interested in </p>
        <p><B>working together?</B></p>
        <p> Fill out the form below, and we will get in touch shortly!</p>
        <p>We can't wait to hear from you!</p>
        <p><strong>Email:</strong> <a href="mailto:shiryonpvtltd@gmail.com">shiryonpvtltd@gmail.com</a></p>
        <p><strong>Phone:</strong> <a href="tel:+919032915050">9032915050</a></p>
      </div>

      <div class="form-box">
        <h2>Register Now</h2>
        <form name="detailsform" method="POST" action="https://formspree.io/f/mnnplnjn">
          <div class="name-fields">
            <input type="text" name="first-name" placeholder="First Name" required />
            <input type="text" name="last-name" placeholder="Last Name" required />
          </div>
          <input type="email" name="email" placeholder="Email Address" required />
          <input type="tel" name="contact-number" placeholder="Contact Number" required />
          <textarea name="message" placeholder="Message" required></textarea>
          <button type="submit">Submit</button>
        </form>
      </div>
    </div>

    <footer>
      <div class="Address"></div>
      <p>SHIRYON TEXTILES PVT LTD,</p>
      <p>Plot 326, First floor, TNGO’s colony phase 2, Gachibowli, Hyderabad, India, 500032.</p>
    </footer>
  </body>
</html>
