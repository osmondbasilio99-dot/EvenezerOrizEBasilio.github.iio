<Index html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TechHeal Registration</title>
  <link rel="icon" href="https://i.pinimg.com/1200x/76/dc/20/76dc20b5b38eef2c3df1c29e4f9e6903.jpg" type="image/png">

  <style>
    body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; margin: 0; text-align: center; background-color: #f0f8ff; }

    /* The Blue Registration Section */
    #registration-section {
      background-color: #1e3a8a;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center; 
    }

    .form-box {
      background: white;
      padding: 30px;
      border-radius: 10px;
      width: 320px;
      text-align: left;
      box-shadow: 0px 4px 15px rgba(0,0,0,0.2);
    }

    h2 { color: #0ea5e9; text-align: center; margin-top: 0; }
    label { font-weight: bold; display: block; margin-top: 15px; }
    input, select, textarea { width: 100%; padding: 10px; margin-top: 5px; box-sizing: border-box; border: 1px solid #ccc; border-radius: 4px; }
    
    button { 
      width: 100%; padding: 12px; margin-top: 20px; 
      background-color: #0ea5e9; color: white; border: none; 
      border-radius: 5px; cursor: pointer; font-weight: bold; transition: background 0.3s;
    }

    button:hover { background-color: #0284c7; }

    /* The Services Section (Hidden at first) */
    #services-section {
      display: none;
      padding: 50px 20px;
      max-width: 800px;
      margin: auto;
    }

    .price { color: #16a34a; font-weight: bold; font-size: 1.2em; }
    ul { list-style: none; padding: 0; }
    li { margin: 20px 0; padding: 20px; border: 1px solid #ddd; border-radius: 8px; background: white; }
    
    .service-img {
      width: 100%;
      max-width: 300px;
      border-radius: 8px;
      margin-top: 10px;
    }
  </style>
</head>
<body>

  <div id="registration-section">
    <div class="form-box">
      <h2>Register</h2>
      <form onsubmit="showServices(); return false;">
        <label>Name:</label>
        <input type="text" placeholder="Enter your name" required>

        <label>Grade Level:</label>
        <select>
          <option>Grade 7-9</option>
          <option>Grade 10-12</option>
        </select>

        <label>Device Issue:</label>
        <textarea placeholder="Describe the problem..." rows="3"></textarea>

        <button type="submit">View Services</button>
      </form>
    </div>
  </div>

  <div id="services-section">
    <h1>TechHeal Gadget Repairs</h1>
    <p style="font-size: 1.2em; color: #555;"><i>"Don't replace it—let us revive it!"</i></p>

    <h3>Our Services:</h3>
    <ul>
      <li>
        <div>Screen Replacement — <span class="price">₱1,200</span></div>
        <img src="https://i.pinimg.com/736x/8d/f4/33/8df43361132034e34190011f0c23940c.jpg" alt="Screen Repair" class="service-img">
      </li>
      
      <li>
        <div>Battery Installation — <span class="price">₱1,500</span></div>
        <img src="https://i.pinimg.com/736x/91/9f/61/919f61b0724618e7d23d9df0d82626e6.jpg" alt="Battery Repair" class="service-img">
      </li>
    </ul>

    <p>Questions? Call us: <a href="tel:5551234" style="color: #0ea5e9; font-weight: bold;">555-1234</a></p>
    
    <button onclick="location.reload()" style="width: auto; padding: 10px 30px; background-color: #64748b;">Back to Home</button>
  </div>

  <script>
    function showServices() {
      document.getElementById("registration-section").style.display = "none";
      document.getElementById("services-section").style.display = "block";
      window.scrollTo(0, 0);
    }
  </script>

</body>
</html>
