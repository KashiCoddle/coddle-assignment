<!-- THIS CODE IS ON KASHINAT.UNNE.143@GMAIL.COM  file as on chatgpt is HTML CSS Layout Design-->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Travel Destination</title>
  <style>
    /* General Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body, html {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 100%;
      height: 100%;
    }

    /* Navbar Styling */
    .navbar {
      width: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 20px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      position: fixed;
      top: 0;
      z-index: 1000;
      background-color: #fff;
    }

    .navbar .logo-container {
      display: flex;
      align-items: center;
    }

    .navbar .logo-container img {
      width: 40px;
      height: 40px;
      margin-right: 10px;
    }

    .navbar .logo-container h2 {
      font-size: 1.5rem;
      color: solid black;
    }

    .navbar ul {
      list-style: none;
      display: flex;
      gap: 50px;
    }

    .navbar ul li {
      font-size: 1rem;
      color: #000;
      cursor: pointer;
      transition: color 0.3s;
    }

    .navbar ul li:hover {
      color: #5c4be0;
    }

    .navbar .auth-buttons {
      display: flex;
      gap: 15px;
    }

    .navbar .auth-buttons .btn {
      padding: 10px 20px;
      border-radius: 20px;
      border: none;
      cursor: pointer;
      font-size: 1rem;
      transition: all 0.3s;
    }

    .navbar .auth-buttons .login {
      background: white;
      color: black;
      border: 2px solid white;
    }

    .navbar .auth-buttons .login:hover {
      background: black;
      color: white;
    }

    .navbar .auth-buttons .signup {
      background: #5c4be0;
      color: #fff;
    }

    .navbar .auth-buttons .signup:hover {
      background: #3b37b1;
    }

    /* Container and Background */
    .container {
      position: relative;
      width: 80%;
      padding: 120px 20px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: transparent;
      z-index: 1;
    }

    .background {
      position: absolute;
      top: 85px;
      left: 500px;
      width: 45%;
      height: 65%;
      background: url('images/images6.jpg') no-repeat center/cover;
      background-size: cover;
      opacity: 0.2;
      z-index: -1;
      clip-path: circle(70% at 50% 50%);
      
      
    }
    

    /* Text Section */
    .text-section {
      max-width: 200%;
      text-align: left;
      z-index: 1;
      margin-right: 300px;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      background: #fff;
      color: #ff3380;
      font-size: 14px;
      padding: 0px 30px;
      border-radius: 30px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      margin-bottom: 10px;
    }

    .badge .icon1 {
      font-size: 1.5rem;
      
    }

    h1 {
      font-size: 3rem;
      line-height: 1.2;
      color: #000;
    }

    h1 .highlight {
      color: #ff3380;
    }

    p {
      color: #777;
      font-size: 1rem;
      margin: 20px 0;
    }

    .buttons {
      margin-top: 20px;
    }

    .btn {
      padding: 10px 20px;
      border: none;
      border-radius: 20px;
      cursor: pointer;
      font-size: 1rem;
    }

    .get-started {
      background-color: #5c4be0;
      color: #fff;
    }

    .watch-demo {
      background-color: white;
      color: black;
      border: 2px white;
    }

    .watch-demo:hover {
      background-color: #5c4be0;
      color: white;
    }

    /* Image Section */
    .image-section {
      position: relative;
      display: flex;
      align-items: center;
      gap: 15px;
      z-index: 2;
      background: transparent;
    }

    .left-images {
      display: flex;
      flex-direction: column;
      gap: 130px;
      width: auto;
      height: auto;
    }

    .image-card {
      position: relative;
      height: 100px;
    }

    .image-card img {
      display: block;
      width: 100%;
      height: -10px;
      left: -100px;
      top: 80px;
      border-radius: 40px;
      position: relative;
      z-index: 2;
    }

    .image-card .logo {
      position: absolute;
      bottom: -110px;
      left: -15px;
      background: rgba(255, 255, 255, 0.8);
      padding: 5px;
      border-radius: 50%;
      width: 40px;
      height: 40px;
      display: flex;
      justify-content: center;
      align-items: center;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
    }

    .image-card .tag {
      position: absolute;
      /* bottom: auto;
      right: auto; */
      background: #fff;
      color: black;
      font-size: 14px;
      padding: 5px 10px;
      border-radius: 15px;
      display: flex;
      align-items: center;
      gap: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      z-index: 3;
    }

    .image-card .tag img {
      width: 20px;
      right: 400px;
      top: 0px;
      
    }

    /* Right Image Centering */
    .right-image {
      display: flex;
      justify-content: center;
      align-items: center;
    }


/* ===============================2nd========================================= */


    /* .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      width: 500%;
      position: relative;
    } */

    /* Left Section: Orange Triangles */
    .triangles {
      position: relative;
      display: flex;
      flex-direction: column;
      gap: 16px;
      margin-top: 100px;
      
    }

    .triangle {
      width: 0;
      height: 0;
      border-left: 10px solid transparent;
      border-right: 10px solid transparent;
      border-bottom: 16px solid orange;
    }

    /* Additional Front Triangles */
    .triangles.front {
      position: absolute;
      left: -10px; /* Offset slightly in front of the existing triangles */
      top: 90px;
    }

    /* Main Section: Logos */
    .logos {
      display: flex;
      gap: 60px;
      flex: 1;
      justify-content: center;
      align-items: center;
    }

    .logos img {
      height: 32px;
      width: auto;
      object-fit: contain;
      margin-top: 100px;
    }

    .logos img:nth-child(3) { /* Smaller for Booking logo */
      height: 28px;
    }

    .logos img:last-child { /* Larger for Orbitz logo */
      height: 40px;
    }

    /* Right Section: Contact Logo */
    .contact-logo {
      position: absolute;
      top: 140px; /* Adjusted for better visibility */
      right: 200px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .circle {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .circle img {
      width: 40px;
      height: 40px;
    }


    /* ==============================3rd===================================== */

    /* Services Section */
    .services {
            padding: 50px 20px;
            background: linear-gradient(to right, #ffffff, #fffbe6);
            display: flex;
            justify-content: center; /* Center content horizontally */
            align-items: center; /* Center content vertically */
            gap: 90px; /* Add space between text and cards */
        }

        /* Left Section Text Styling */
        .services-header {
            max-width: 40%;
            text-align: left;
        }

        .services-header h5 {
            color: #ff007a;
            font-size: 16px;
            text-transform: uppercase;
            margin-bottom: 10px;
        }

        .services-header h1 {
            color: #000;
            font-size: 32px;
            font-weight: bold;
        }

        /* Cards Container */
        .services-kards {
            display: flex;
            gap: 20px; /* Space between cards */
            justify-content: flex-start;
            flex-wrap: wrap; /* Allow cards to wrap on smaller screens */
            width: 650px;
            height: 270px;
        }

        /* Individual Card Styling */
        .kard {
            display: flex;
            flex-direction: column; /* Stack icon and text vertically */
            align-items: center; /* Center align the content within the card */
            background: #fff;
            border-radius: 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 50px 10px 50px 10px;
            width: 200px; /* Set a fixed width for consistent card size */
            height: 240px;
            text-align: center; /* Center align the text */
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
        }

        .icon1 img {
            width: 50px;
            height: 50px;
            margin-bottom: 20px; /* Space between the icon and text */
        }

        .text h3 {
            font-size: 18px;
            color: #000;
            margin-bottom: 10px;
        }

        .text p {
            font-size: 14px;
            color: #666;
        }
    


/* ===========================4th=========================================== */

.container1 {
            max-width: 500px;
            max-height: 450px;
            margin: 0 auto;
            text-align: left;
            position: relative;
        }

        .title {
            color: #FF6090;
            font-size: 14px;
            text-transform: uppercase;
            font-weight: bold;
            margin-bottom: 20px; /* Gap between title and subtitle */
            margin-left: -180px;
        }

        .subtitle {
            color: #000;
            font-size: 28px;
            font-weight: bold;
            margin-bottom: 50px; /* Gap between subtitle and cards */
            margin-left: -180px;
        }

        .cards1 {
            display: flex;
            margin-top: -20px;
            margin-left: -175px;
            gap: 30px; /* Adjusted gap between cards */
        }

        .card2 {
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            width: 400%;
            height: 400px;
            
        }

        .card2 img {
            width: 100%;
            height: 180px; 
            object-fit: cover;
        }

        .card2-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px 15px;
        }

        .card2-title {
            font-size: 16px;
            font-weight: bold;
            color: #000;
        }

        .card2-price {
            color: #FF6090;
            font-size: 16px;
            font-weight: bold;
            text-align: right;
        }

        .card2-content {
            padding: 15px;
            text-align: left;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            height: calc(100% - 210px); /* Adjusted height for the card content */
        }

        .card2-description {
            color: #666;
            font-size: 14px;
            margin-bottom: 40px;
        }

        .card2-rating {
            display: flex;
            align-items: center;
            color: #FFA500;
            font-size: 14px;
            margin-top: -45%;
        }

        .card2-rating .star {
            margin-left: -27px;
            margin-top: -210px;
        }

        .navigation {
            position: absolute;
            top: 20px; 
            right: 20px; 
            display: flex;
            gap: 15px;
        }

        .nav-button {
            width: 40px;
            height: 40px;
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 50%;
            background-color: #f0f0f0;
            color: #000;
            font-size: 18px;
            cursor: pointer;
        }

        .nav-button.active {
            background-color: #6A5ACD;
            color: #fff;
        }

        .decorative {
            position: absolute;
            right: -100px;
            top: 74px;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .decorative .row {
            display: flex;
            justify-content: flex-start;
            gap: 10px;
        }

        .decorative span {
            display: inline-block;
            color: #FFCC00;
            font-size: 24px;
        }



/* ================================5th====================================== */


.travel-container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      width: 150%;
      max-width: 1320px;
      border-radius: 20px;
      top: 100px;
      overflow: hidden;
      padding: 250px 100px 250px 100px;
      box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
      background-color: #ffffff;
      position: relative;
    }

    /* Gradient Circles */
    .gradient-circle {
      position: absolute;
      border-radius: 50%;
      z-index: 1;
      opacity: 0.6;
    }

    .circle1 {
      width: 70px;
      height: 70px;
      top: -10px;
      left: 350px;
      background: radial-gradient(circle, #DF6AAE, #A456B4, #7B52BF);
    }

    .circle2 {
      width: 10px;
      height: 10px;
      bottom: 250px;
      right: 72%;
      background: radial-gradient(circle, #ff5733, rgba(0, 0, 0, 0));
    }

    .circle3 {
      width: 20px;
      height: 20px;
      top: 100px;
      right: 61%;
      background: radial-gradient(circle, #ff5733, rgba(0, 0, 0, 0));
    }

    .circle4 {
      width: 25px;
      height: 25px;
      bottom: 350px;
      left: 5%;
      background: radial-gradient(circle, #DF6AAE, #A456B4, #7B52BF);
    }

    .circle5 {
      width: 30px;
      height: 30px;
      top: 230px;
      right: 68%;
      background: radial-gradient(circle, #ff5733, rgba(0, 0, 0, 0));
    }

    .background-capsule {
      position: absolute;
      top: 50%;
      left: -800px;
      width: 100%;
      height: 300px;
      background-color: #facd49;
      border-radius: 150px / 50%;
      transform: translateY(-50%);
      z-index: 0;
    }

    .left-section {
      position: relative;
      flex: 1;
      z-index: 2;
    }

    .image-wrapper {
      position: relative;
      text-align: center;
    }

    .backpacker-img {
      width: 100%;
      top: -30px;
      right: 45px;
      height: 380px;
      max-width: none;
      z-index: 2;
      position: relative;
    }

    .discount-badge {
      position: absolute;
      top: 12%;
      right: 18%;
      background-color: white;
      color: black;
      padding: 5px 15px;
      border-radius: 50px;
      font-size: 14px;
      font-weight: bold;
      display: flex;
      align-items: center;
      gap: 5px;
      box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
      z-index: 2;
    }

    .discount-badge img {
      width: 30px;
      height: 25px;
    }

    .right-section {
      flex: 1;
      padding: 30px;
    }

    .travel-point {
      font-size: 20px;
      color: #f633bf;
      font-weight: bold;
      margin-bottom: 10px;
      text-align: left;
    }

    .travel-heading {
      font-size: 28px;
      color: #333;
      margin-bottom: 15px;
    }

    .travel-subtext {
      font-size: 16px;
      color: #555;
      line-height: 1.5;
      margin-bottom: 20px;
    }

    .stats {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: space-between;
    }

    .stat-item {
      flex: 1 1 calc(50% - 20px);
      min-width: 150px;
      text-align: center;
    }

    .stat-item strong {
      
      font-size: 24px;
      color: #f56d50;
      margin-bottom: 5px;
    }

    .stat-item {
      flex: 1 1 calc(50% - 20px);
    min-width: 10px;
    text-align: center;
    position: relative;
    background-color: white; /* White background */
    padding: 20px; /* Padding around the text */
    width: 5px;
    height: 100px;
    border-radius: 10px; /* Rounded corners */
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Subtle shadow for elevation */
    margin: 10px 0;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    }

    .luxury-hotel-icon {
      position: absolute;
      bottom: 80px;
      right: -60px;
    display: inline-flex;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #facd49; /* Yellow background */
    border-radius: 50%; /* Circle shape */
    width: 80px; /* Size of the circle */
    height: 80px; /* Size of the circle */
  }

    .luxury-hotel-icon img {
      width: 50px;
      height: 50px;
    }


/* ================================6th====================================== */


/* .container {
      display: flex;
      max-width: 1200px;
      width: 100%;
      gap: 2rem;
      padding: 2rem;
    } */

    /* Left Section */
    .left-section {
      flex: 1;
    }

    .subheading {
      color: #ff4081;
      text-transform: uppercase;
      font-size: 1rem;
      margin-bottom: 0.5rem;
    }

    h1 {
      font-size: 2.5rem;
      color: #333;
      margin-bottom: 1rem;
    }

    .description {
      color: #666;
      font-size: 1rem;
      line-height: 1.5;
      margin-bottom: 2rem;
    }

    .features {
      display: flex;
      flex-direction: column;
      gap: 1.5rem;
    }

    .feature-item {
      display: flex;
      align-items: center;
      gap: 1rem;
    }

    .icon {
      width: 50px;
      height: 50px;
      border-radius: 8px;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .icon img {
      width: 60%;
      height: auto;
    }

    .orange {
      background-color: orange;
    }

    .yellow {
      background-color: yellow;
    }

    .pink {
      background-color: pink;
    }

    /* Right Section */
    .right-section {
      flex: 1;
      position: relative;
    }

    .capsule-image {
      width: 220px;
      height: 350px;
      border-radius: 120px; /* Smooth corners with straight sides */
      object-fit: cover;
      position: absolute;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .capsule-image.main {
      position: relative;
      margin-top: 10%;
      left: 10%;
      z-index: 1;
    }

    .capsule-image.secondary {
      width: 175px;
      height: 240px;
      top: 45%;
      left: 30%;
      z-index: 2;
      border: 10px solid #fff;
    }

    .image-overlay {
      position: relative;
    }

    /* Decorative Text and Icon on Image */
    .image-text {
      position: absolute;
      top: 25%; /* Adjust as needed */
      right: 35%; /* Adjust as needed */
      display: flex;
      align-items: center;
      gap: 0.5rem;
      background: rgba(255, 255, 255, 0.8);
      padding: 0.3rem 0.8rem;
      border-radius: 20px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
      z-index: 1;
    }

    .image-text img {
      width: 20px;
      height: 20px;
      border-radius: 50%;
    }

    .image-text span {
      font-size: 0.8rem;
      font-weight: bold;
      color: #333;
    }

    .decorative-x {
  position: absolute;
  top: -400px;
  right: -40%;
  width: 200px;  /* Circle diameter */
  height: 160px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  
}

.x-piece {
  position: absolute;
  font-size: 0.75rem;  /* Adjust font size to fit the circle */
  font-weight: bold;
  color: yellow;
}

/* Adjust positions to form a proper circle */
.x-piece:nth-child(1) { top: 0%; left: 50%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(2) { top: 14%; left: 85%; transform: translateX(-50%) translateY(-70%); }
.x-piece:nth-child(3) { top: 30%; left: 95%; transform: translateX(-50%) translateY(-40%); }
.x-piece:nth-child(4) { top: 50%; left: 100%; transform: translateX(-50%) translateY(-20%); }
.x-piece:nth-child(5) { top: 70%; left: 95%; transform: translateX(-50%) translateY(10%); }
.x-piece:nth-child(6) { top: 85%; left: 85%; transform: translateX(-50%) translateY(40%); }
.x-piece:nth-child(7) { top: 100%; left: 50%; transform: translateX(-50%) translateY(70%); }
.x-piece:nth-child(8) { top: 85%; left: 15%; transform: translateX(-50%) translateY(40%); }
.x-piece:nth-child(9) { top: 70%; left: 5%; transform: translateX(-50%) translateY(10%); }
.x-piece:nth-child(10) { top: 50%; left: 0%; transform: translateX(-50%) translateY(-20%); }
.x-piece:nth-child(11) { top: 30%; left: 5%; transform: translateX(-50%) translateY(-40%); }
.x-piece:nth-child(12) { top: 14%; left: 15%; transform: translateX(-50%) translateY(-70%); }

.x-piece:nth-child(13) { top: 14%; left: 50%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(14) { top: 14%; left: 40%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(15) { top: 14%; left: 30%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(16) { top: 14%; left: 22%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(17) { top: 14%; left: 60%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(18) { top: 14%; left: 70%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(19) { top: 25%; left: 50%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(20) { top: 25%; left: 40%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(21) { top: 25%; left: 30%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(22) { top: 100%; left: 22%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(23) { top: 25%; left: 10%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(24) { top: 25%; left: 60%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(25) { top: 25%; left: 70%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(26) { top: 25%; left: 80%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(27) { top: 25%; left: 18%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(28) { top: 35%; left: 18%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(29) { top: 35%; left: 27%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(30) { top: 35%; left: 37%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(31) { top: 35%; left: 47%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(32) { top: 35%; left: 57%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(33) { top: 35%; left: 67%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(34) { top: 35%; left: 77%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(35) { top: 40%; left: 47%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(36) { top: 40%; left: 37%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(37) { top: 40%; left: 27%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(38) { top: 40%; left: 18%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(39) { top: 40%; left: 8%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(40) { top: 40%; left: -3%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(41) { top: 40%; left: 57%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(42) { top: 35%; left: 15%; transform: translateX(-50%) translateY(-100%); }
.x-piece:nth-child(43) { top: 40%; left: 67%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(44) { top: 40%; left: 77%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(45) { top: 40%; left: 87%; transform: translateX(50%) translateY(-40%); }
.x-piece:nth-child(46) { top: 100%; left: 46%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(47) { top: 100%; left: 36%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(48) { top: 100%; left: 26%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(49) { top: 100%; left: 56%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(50) { top: 100%; left: 65%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(51) { top: 100%; left: 73%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(52) { top: 15%; left: 73%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(53) { top: 3%; left: 56%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(54) { top: 4%; left: 66%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(55) { top: 13%; left: 73%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(56) { top: 30%; left: 85%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(57) { top: 1%; left: 35%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(58) { top: 1%; left: 26%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(59) { top: 4%; left: 18%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(60) { top: 70%; left: 47%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(61) { top: 70%; left: 37%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(62) { top: 70%; left: 27%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(63) { top: 70%; left: 17%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(64) { top: 70%; left: 7%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(65) { top: 70%; left: -4%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(66) { top: 70%; left: 57%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(67) { top: 70%; left: 67%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(68) { top: 70%; left: 77%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(69) { top: 70%; left: 85%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(70) { top: 70%; left: 92%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(71) { top: 80%; left: 27%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(72) { top: 80%; left: 37%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(73) { top: 80%; left: 47%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(74) { top: 80%; left: 17%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(75) { top: 80%; left: 7%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(76) { top: 80%; left: 57%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(77) { top: 80%; left: 67%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(78) { top: 80%; left: 77%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(79) { top: 80%; left: 84%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(80) { top: 90%; left: 47%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(81) { top: 90%; left: 37%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(82) { top: 90%; left: 27%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(83) { top: 90%; left: 17%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(84) { top: 90%; left: 7%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(85) { top: 90%; left: 57%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(86) { top: 90%; left: 67%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(87) { top: 90%; left: 77%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(88) { top: 90%; left: 87%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(89) { top: 100%; left: 73%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(90) { top: 58%; left: 57%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(91) { top: 58%; left: 67%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(92) { top: 58%; left: 77%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(93) { top: 58%; left: 87%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(94) { top: 58%; left: 37%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(95) { top: 58%; left: 27%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(96) { top: 58%; left: 17%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(97) { top: 58%; left: 7%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(98) { top: 112%; left: 56%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(99) { top: 111%; left: 66%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(100) { top: 109%; left: 76%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(101) { top: 111%; left: 36%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(102) { top: 111%; left: 26%; transform: translateX(50%) translateY(-100%); }
.x-piece:nth-child(103) { top: 45%; left: 95%; transform: translateX(50%) translateY(-100%); }


    .decorative-lines {
      position: absolute;
      top: 5%; /* Spread the circle wider */
      margin-top: -20px;
      right: 45%;
      width: 180px;
      height: 180px;
      background: transparent;
      border-radius: 50%;
      display: grid;
      place-items: center;
    }

    .line-piece {
      width: 4px;
      height: 12px;
      background-color: #ff4081;
      position: absolute;
      transform-origin: center bottom;
    }

    /* Rotate pieces to form a fuller circle */
    .line-piece:nth-child(1) { transform: rotate(0deg) translate(0, -80px); }
    .line-piece:nth-child(2) { transform: rotate(15deg) translate(0, -80px); }
    .line-piece:nth-child(3) { transform: rotate(30deg) translate(0, -80px); }
    .line-piece:nth-child(4) { transform: rotate(45deg) translate(0, -80px); }
    .line-piece:nth-child(5) { transform: rotate(60deg) translate(0, -80px); }
    .line-piece:nth-child(6) { transform: rotate(75deg) translate(0, -80px); }
    .line-piece:nth-child(7) { transform: rotate(90deg) translate(0, -80px); }
    .line-piece:nth-child(8) { transform: rotate(105deg) translate(0, -80px); }
    .line-piece:nth-child(9) { transform: rotate(120deg) translate(0, -80px); }
    .line-piece:nth-child(10) { transform: rotate(135deg) translate(0, -80px); }
    .line-piece:nth-child(11) { transform: rotate(150deg) translate(0, -80px); }
    .line-piece:nth-child(12) { transform: rotate(165deg) translate(0, -80px); }
    .line-piece:nth-child(13) { transform: rotate(180deg) translate(0, -80px); }
    .line-piece:nth-child(14) { transform: rotate(195deg) translate(0, -80px); }
    .line-piece:nth-child(15) { transform: rotate(210deg) translate(0, -80px); }
    .line-piece:nth-child(16) { transform: rotate(225deg) translate(0, -80px); }
    .line-piece:nth-child(17) { transform: rotate(240deg) translate(0, -80px); }
    .line-piece:nth-child(18) { transform: rotate(255deg) translate(0, -80px); }
    .line-piece:nth-child(19) { transform: rotate(270deg) translate(0, -80px); }
    .line-piece:nth-child(20) { transform: rotate(285deg) translate(0, -80px); }
    .line-piece:nth-child(21) { transform: rotate(300deg) translate(0, -80px); }
    .line-piece:nth-child(22) { transform: rotate(315deg) translate(0, -80px); }
    .line-piece:nth-child(23) { transform: rotate(330deg) translate(0, -80px); }
    .line-piece:nth-child(24) { transform: rotate(345deg) translate(0, -80px); }


/* ================================7th====================================== */


/* Testimonial Section Styling */
.testimonial-section {
      text-align: center;
      /* background: linear-gradient(to right, #f8f3fc, #ffffff); */
      padding: 50px;
      /* border-radius: 10px; */
      /* box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1); */
      width: 80%;
      max-width: 900px;
    }

    /* Title and Subtitle */
    .testimonial-title {
      color: #ff8eb3;
      font-size: 1.2rem;
      letter-spacing: 2px;
      margin-bottom: 10px;
    }

    .testimonial-subtitle {
      font-size: 1.8rem;
      font-weight: bold;
      color: #333;
      margin-bottom: 30px;
    }

    /* Testimonial Container */
    .testimonial-container {
      display: flex;
      align-items: center;
      position: relative;
    }

    .nav-arrow {
      background: #ffffff;
      border: none;
      font-size: 2rem;
      padding: 10px;
      cursor: pointer;
      border-radius: 50%;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    .nav-arrow.left-arrow {
      position: absolute;
      left: -40px;
      background: #ffffff;
      color: #000;

    }

    .nav-arrow.right-arrow {
      position: absolute;
      right: -40px;
      background: #5d50c6;
      color: #ffffff;
    }

    /* Testimonial Content */
    .testimonial-content {
      flex: 1;
      text-align: center;
    }

    .client-image {
      margin: 0 auto 20px;
      width: 80px;
      height: 80px;
      border-radius: 50%;
      background: #ffcf85;
      overflow: hidden;
    }

    .client-image img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .client-name {
      font-size: 1.2rem;
      font-weight: bold;
      margin: 10px 0;
      color: #ff8b3d;
    }

    .client-name span {
      font-weight: normal;
      color: #777;
    }

    .rating {
      color: #ffc107;
      font-size: 1.5rem;
      margin: 10px 0;
    }

    .testimonial-text {
      font-size: 0.9rem;
      color: #555;
      line-height: 1.6;
      max-width: 600px;
      margin: 0 auto;
    }

    /* Pagination Dots */
    .pagination {
      margin-top: 20px;
    }

    .dot {
      width: 10px;
      height: 10px;
      margin: 0 5px;
      background: #ccc;
      border-radius: 50%;
      display: inline-block;
      cursor: pointer;
    }

    .dot.active {
      background: #ff8eb3;
    }


/* ================================8th====================================== */


.newsletter-container {
      text-align: center;
      padding: 5rem;
      background-color: #FFF8F0;
      position: relative;
      border-radius: 10px;
      width: 90%;
      max-width: 700px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .pattern-top-left {
      position: absolute;
      top: -30px;
      left: -30px;
      width: 100px;
      height: 100px;
      background: url('images/Picsart_24-12-29_17-18-56-390.png') no-repeat center/contain; /* Replace with your dot triangle image path */
    }

    .bottom-right-design {
      position: absolute;
      bottom: -250px;
      right: -330px;
      width: 50px; /* Adjust size as needed */
      height: auto;
      z-index: -1; /* Ensures the design stays behind content */
    }

    .newsletter-title {
      color: #FF6F91;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      font-size: 14px;
      margin-bottom: 1rem;
    }

    .main-heading {
      font-size: 24px;
      font-weight: bold;
      margin-bottom: 2rem;
      line-height: 1.5;
    }

    .subscription-form {
      display: flex;
      justify-content: center;
    }

    .input-container {
      position: relative;
      display: flex;
      gap: 10px;
    }

    input[type="email"] {
      padding: 10px 15px 10px 40px; /* Add padding for the icon */
      border: 1px solid #ddd;
      border-radius: 25px;
      flex: 1;
      font-size: 16px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .email-icon {
      position: absolute;
      top: 50%;
      left: 15px;
      transform: translateY(-50%);
      width: 20px;
      height: 20px;
    }

    button {
      background-color: #6A5ACD;
      color: #fff;
      padding: 10px 20px;
      border: none;
      border-radius: 25px;
      font-size: 16px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #483D8B;
    }




    


/* ================================9th====================================== */    


 /* General Footer Styling */
 .footer1 {
  background-color: #f9f9f9;
  color: #333;
  font-family: Arial, sans-serif;
  padding: 150px ;
  
}

.footer1-container {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  max-width: 1200px;
  margin: 0 auto;
}

.footer1-left, 
.footer1-middle, 
.footer1-right {
  flex: 1;
  margin: 30px;
}

 .footer1-logo {
  display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      font-weight: bold;
      font-size: 16px;
      margin-bottom: 1rem;
}

.footer1-logo img {
      width: 20px; /* Adjust logo size */
      height: 20px;
      margin-left: -30%;
      
    }



/* Left Section Styling */
.footer1-left p {
  line-height: 1.6;
  font-size: 14px;
}

/* Middle Section Styling */
.footer1-middle {
  display: flex;
  gap: 10px; /* Space between columns */
}

.footer1-middle .column {
  flex: 1;
  margin: 30px;
}

.footer1-middle h4 {
  font-size: 16px;
  font-weight: bold;
  margin-bottom: 10px;
}

.footer1-middle ul {
  list-style-type: none;
  padding: 0;
}

.footer1-middle ul li {
  margin: 8px 0;
}

.footer1-middle ul li a {
  text-decoration: none;
  color: #333;
  font-size: 14px;
  transition: color 0.3s;
}

.footer1-middle ul li a:hover {
  color: #6a5acd; /* Purple hover effect */
}

/* Right Section Styling */
.footer1-right h4 {
  font-size: 16px;
  font-weight: bold;
  margin-bottom: 10px;
}

.footer1-right p {
  margin: 8px 0;
  font-size: 14px;
}

.footer1-right a {
  text-decoration: none;
  color: #333;
  transition: color 0.3s;
}

.footer1-right a:hover {
  color: #6a5acd;
}

/* Social Media Icons */
.footer1-social {
  text-align: center; 
  margin-left: -600px;
  margin-top: 20px;
  
}

.footer1-social a {
  margin: 0 10px;
  display: inline-block;
}

.footer1-social img {
  width: 20px;
  height: 20px;
  transition: transform 0.3s;
  
}

.footer1-social img:hover {
  transform: scale(1.1);
}



  </style>
</head>
<body>
  <!-- Navbar -->
  <div class="navbar">
    <div class="logo-container">
      <img src="images/images.jpg" alt="Site Logo">
      <h2>Travlog</h2>
    </div>
    <ul>
      <li>Home</li>
      <li>Destinations</li>
      <li>About Us</li>
      <li>Contact</li>
    </ul>
    <div class="auth-buttons">
      <button class="btn login">Login</button>
      <button class="btn signup">Signup</button>
    </div>
  </div>

  <!-- Main Content -->
  <div class="container">
    <div class="background"></div>

    <!-- Text Section -->
    <div class="text-section">
      <div class="badge">
        <span class="icon1">Explore the world!🎁</span>
      </div>
      <h1>
        Travel <span class="highlight">top destination</span><br> of the world
      </h1>
      <p>We always make our customer happy by providing as many choices as possible</p>
      <div class="buttons">
        <button class="btn get-started">Get Started</button>
        <button class="btn watch-demo">Watch Demo</button>
      </div>
    </div>

    <!-- Image Section -->
    <div class="image-section">
      <!-- Left Images -->
      <div class="left-images">
        <div class="image-card">
          <img src="images/images3.jpg" alt="Destination 1">
          <div class="logo">
            <img src="images/telegram-image.jpg" alt="Telegram Logo">
          </div>
        </div>
        
        <div class="image-card">
          <img src="images/images4.jpg" alt="Destination 2">
        </div>
      </div>

      <!-- Right Image -->
      <div class="right-image">
        <div class="image-card">
          <img src="images/images5.jpg" alt="Destination 3">
          <div class="tag">
            <img src="images/location-image.png" alt="Location">Top Places
          </div>
        </div>
      </div>
    </div>
  </div>



<!-- ==========================2nd HTML=================================-->


  <div class="container">
    <!-- Left Section: Original Orange Triangles -->
    <div class="triangles">
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
    </div>

    <!-- Left Section: Additional Front Triangles -->
    <div class="triangles front">
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
      <div class="triangle"></div>
    </div>

    <!-- Main Section: Logos -->
    <div class="logos">
      <img src="images/tripadvisor1.png" alt="Tripadvisor">
      <img src="images/Expedia.png" alt="Expedia">
      <img src="images/booking.png" alt="Booking.com">
      <img src="images/airbnb1.png" alt="Airbnb">
      <img src="images/orbitz2.png" alt="Orbitz">
    </div>

    <!-- Right Section: Contact Logo -->
    <div class="contact-logo">
      <div class="circle">
        <img src="images/contact.png" alt="Contact">
      </div>
    </div>
  </div>



<!-- ==========================3rd HTML=================================-->

  <section class="services">
    <!-- Text Section -->
    <div class="services-header">
        <h5>SERVICES</h5>
        <h1>Our top value <br>categories for you</h1>
    </div>
    
    <!-- Cards Section -->
    <div class="services-kards">
        <!-- Card 1 -->
        <div class="kard">
            <div class="icon1">
                <img src="images/world-icon.png" alt="Tour Guide Icon">
            </div>
            <div class="text">
                <h3>Best Tour Guide</h3>
                <p>What looked like a small <br>patch of purple grass,<br> above five feet.</p>
            </div>
        </div>
        <!-- Card 2 -->
        <div class="kard">
            <div class="icon1">
                <img src="images/easy-booking.jpg" alt="Easy Booking Icon">
            </div>
            <div class="text">
                <h3>Easy Booking</h3>
                <p>Square, was moving <br> across the sand in their <br> direction.</p>
            </div>
        </div>
    </div>
</section>



<!-- ==========================4th HTML=================================-->


<div class="container1">
  <p class="title">Top Destination</p>
  <h1 class="subtitle">Explore top destination</h1>

  <div class="cards1">
      <!-- Card 1 -->
      <div class="card2">
          <img src="images/beach.jfif" alt="Paradise Beach">
          <div class="card2-header">
              <p class="card2-title">Paradise Beach,<br> Bantayan Island</p>
              <p class="card2-price">$550.16</p>
          </div>
          <div class="card2-content">
              <p class="card2-description">Rome, Italy</p>
              <div class="card2-rating">
                   <span class="star">&#9733;  4.8⭐</span> 
              </div>
          </div>
      </div>

      <!-- Card 2 -->
      <div class="card2">
          <img src="images/fish.jfif" alt="Ocean full of colors">
          <div class="card2-header">
              <p class="card2-title">Ocean with full of <br>Colors</p>
              <p class="card2-price">$20.99</p>
          </div>
          <div class="card2-content">
              <p class="card2-description">Maldives</p>
              <div class="card2-rating">
                   <span class="star">&#9733; 4.5⭐</span>
              </div>
          </div>
      </div>

      <!-- Card 3 -->
      <div class="card2">
          <img src="images/cloud.jfif" alt="Mountain View">
          <div class="card2-header">
              <p class="card2-title">Mountain View,<br> Above the cloud</p>
              <p class="card2-price">$150.99</p>
          </div>
          <div class="card2-content">
              <p class="card2-description">United Arab Emirates</p>
              <div class="card2-rating">
                    <span class="star">&#9733; 5.0⭐</span> 
              </div>
          </div>
      </div>
  </div>

  <div class="navigation">
      <div class="nav-button">&#8592;</div>
      <div class="nav-button active">&#8594;</div>
  </div>

  <div class="decorative">
      <div class="row">
          <span>&#10006;</span>
      </div>
      <div class="row">
          <span>&#10006;</span>
          <span>&#10006;</span>
      </div>
      <div class="row">
          <span>&#10006;</span>
          <span>&#10006;</span>
          <span>&#10006;</span>
      </div>
  </div>
</div>


<!-- ==========================5th HTML=================================-->


<div class="travel-container">
  <!-- Gradient Circles -->
  <div class="gradient-circle circle1"></div>
  <div class="gradient-circle circle2"></div>
  <div class="gradient-circle circle3"></div>
  <div class="gradient-circle circle4"></div>
  <div class="gradient-circle circle5"></div>

  <!-- Background Design -->
  <div class="background-capsule"></div>

  <!-- Left Section -->
  <div class="left-section">
    <div class="image-wrapper">
      <img src="images/file.png" alt="Traveler" class="backpacker-img">
      <div class="discount-badge">
        <img src="images/discount-image.jpg" alt="Discount Icon"> Discounted Price
      </div>
    </div>
  </div>

  <!-- Right Section -->
  <div class="right-section">
    <h1 class="travel-point">Travel Point</h1>
    <h2 class="travel-heading">We helping you find your dream location</h2>
    <p class="travel-subtext">
      Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC.
    </p>
    <div class="stats">
      <div class="stat-item">
        <strong>500+</strong><br>Holiday Package
      </div>
      <div class="stat-item">
        <strong>100</strong><br>
        Luxury Hotel
        <span class="luxury-hotel-icon">
          <img src="images/hotel.png" alt="Hotel Icon">
        </span>
      </div>
      <div class="stat-item">
        <strong>7</strong><br>Premium Airlines
      </div>
      <div class="stat-item">
        <strong>2k+</strong><br>Happy Customer
      </div>
    </div>
  </div>
</div>


<!-- ==========================6th HTML=================================-->


<div class="container">
  <!-- Left Section -->
  <div class="left-section">
    <p class="subheading">Key Features</p>
    <h1>We offer the best services</h1>
    <p class="description">
      Contrary to popular belief, Lorem Ipsum is not simply random text. It has
      roots in a piece of classical Latin literature from 45 BC.
    </p>

    <!-- Feature List -->
    <div class="features">
      <div class="feature-item">
        <div class="icon orange">
          <img src="images/image-location-icon-6.jpg" alt="Service Icon">
        </div>
        <div class="text">
          <h3>We offer best services</h3>
          <p>Lorem Ipsum is not simply random text</p>
        </div>
      </div>
      <div class="feature-item">
        <div class="icon yellow">
          <img src="images/calender-image.png" alt="Calendar Icon">
        </div>
        <div class="text">
          <h3>Schedule your trip</h3>
          <p>It has roots in a piece of classical</p>
        </div>
      </div>
      <div class="feature-item">
        <div class="icon pink">
          <img src="images/discounted-coupen.png" alt="Coupon Icon">
        </div>
        <div class="text">
          <h3>Get discounted coupons</h3>
          <p>Lorem Ipsum is not simply random text</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Right Section -->
  <div class="right-section">
    <div class="image-overlay">
      <img src="images/church-image.jpg" alt="Church" class="capsule-image main">
      <!-- Decorative Text with Icon -->
      <div class="image-text">
        <img src="images/Google Maps icon.jpg" alt="Earth Icon">
        <span>Paradise on Earth</span>
      </div>
      <!-- Decorative Patterns -->
      <div class="decorative-x">
          <div class="x-line">
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            <span class="x-piece">X</span>
            </div> 
      </div>

      <div class="decorative-lines">
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
        <div class="line-piece"></div>
      </div>
    </div>
    <img src="images/sky-dying.jpg" alt="Water" class="capsule-image secondary">
  </div>
</div>


<!-- ==========================7th HTML=================================-->


<div class="testimonial-section">
  <h2 class="testimonial-title">TESTIMONIALS</h2>
  <h3 class="testimonial-subtitle">Trust our clients</h3>

  <div class="testimonial-container">
    <!-- Left Arrow -->
    <button class="nav-arrow left-arrow">&larr;</button>

    <!-- Testimonial Content -->
    <div class="testimonial-content">
      <div class="client-image">
        <img src="images/lens.jpg" alt="Client with VR Goggles">
      </div>
      <h4 class="client-name">Mark Smith <span>/ Travel Enthusiast</span></h4>
      <div class="rating">
        <span>★</span><span>★</span><span>★</span><span>★</span><span>★</span>
      </div>
      <p class="testimonial-text">
        Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC.
      </p>
    </div>

    <!-- Right Arrow -->
    <button class="nav-arrow right-arrow">&rarr;</button>
  </div>

  <!-- Pagination Dots -->
  <div class="pagination">
    <span class="dot"></span>
    <span class="dot active"></span>
    <span class="dot"></span>
  </div>
</div>


<!-- ==========================8th HTML=================================-->


<div class="newsletter-container">
  <div class="pattern-top-left"></div>
  <h3 class="newsletter-title">SUBSCRIBE TO OUR NEWSLETTER</h3>
  <h1 class="main-heading">Prepare yourself & let’s explore the beauty of the world</h1>
  <form class="subscription-form">
    <div class="input-container">
      <img src="images/email.png" alt="Email Icon" class="email-icon"> <!-- Replace with your email icon image -->
      <input type="email" placeholder="Your Email" required>
      <button type="submit">Subscribe</button>
    </div>
  </form>
  <img src="images/heroobj-2582171a.svg" alt="Decorative Design" class="bottom-right-design">
</div>



<!-- ==========================9th HTML=================================-->


<footer class="footer1">
  <div class="footer1-container">
    <!-- Left Section -->
    <div class="footer1-left">
      <div class="footer1-logo">
        <img src="images/images.jpg" alt="Travlog Logo"> <!-- Replace with your Travlog logo image -->
        Travlog
      </div>
      <p>
        Contrary to popular belief,<br> Lorem Ipsum is not simply <br> random text. 
        It has roots <br> in a piece of classical Latin <br> literature from 45 BC.
      </p>
    </div>

    <!-- Middle Section -->
    <div class="footer1-middle">
      <div class="column">
        <h4>Company</h4>
        <ul>
          <li><a href="#">About</a></li>
          <li><a href="#">Career</a></li>
          <li><a href="#">Mobile</a></li>
        </ul>
      </div>
      <div class="column">
        <h4>Resources</h4>
        <ul>
          <li><a href="#">Why Travlog?</a></li>
          <li><a href="#">Partner with us</a></li>
          <li><a href="#">FAQs</a></li>
          <li><a href="#">Blog</a></li>
        </ul>
      </div>
    </div>

    <!-- Right Section -->
    <div class="footer1-right">
      <h4>Contact</h4>
      <p>+00 92 1234 56789</p>
      <p><a href="mailto:info@travlog.com">info@travlog.com</a></p>
      <p>205. R Street, New York</p>
      <p>BD23200</p>
    </div>
  </div>

  <!-- Social Media Icons -->
  <div class="footer1-social">
    <a href="#"><img src="images/facebook.jpg" alt="Facebook"></a>
    <a href="#"><img src="images/tweeter.png" alt="Twitter"></a>
    <a href="#"><img src="images/instagram.jpg" alt="Instagram"></a>
  </div>
</footer>



</body>
</html>





