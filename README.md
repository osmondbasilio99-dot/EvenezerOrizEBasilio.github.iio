<!DOCTYPE html>
<html>
<head>
  <title>TechHeal Registration</title>
  <link rel="icon" href="https://i.pinimg.com/1200x/76/dc/20/76dc20b5b38eef2c3df1c29e4f9e6903.jpg"  type="image/png">
 

  <style>
    body { font-family: sans-serif; margin: 0; text-align: center; background-color: #f0f8ff; }

    /* The Blue Registration Section */
    #registration-section {
      background-color: #1e3a8a;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center; }

    .form-box {
      background: white;
      padding: 30px;
      border-radius: 10px;
      width: 300px;
      text-align: left; }
    h2 { color: #0ea5e9; text-align: center; }
    label { font-weight: bold; display: block; margin-top: 10px; }
     input, select, textarea { width: 100%; padding: 8px; margin-top: 5px; box-sizing: border-box; }
 button { 
      width: 100%; padding: 10px; margin-top: 20px; 
      background-color: #0ea5e9; color: white; border: none; 
      border-radius: 5px; cursor: pointer; font-weight: bold; }

    /* The Services Section (Hidden at first) */
    #services-section {
      display: none;
      padding: 50px; }

    .price { color: green; font-weight: bold; }
    ul { list-style: none; padding: 0; }
    li { margin: 10px; padding: 10px; border-bottom: 1px solid #ddd; }
  </style>
</head>
<body>

  <div id="registration-section">
    <div class="form-box">
      <h2>Register</h2>
      <form onsubmit="showServices(); return false;">
        <label>Name:</label>
        <input type="text" required>

        <label>Grade Level:</label>
        <select>
          <option>Grade 7-9</option>
          <option>Grade 10-12</option>
        </select>

        <label>Device Issue:</label>
        <textarea></textarea>

        <button type="submit">View Services</button>
      </form>
    </div>
  </div>

  <div id="services-section">
    <h1>TechHeal Gadget Repairs</h1>
    <p><i>"Don't replace it—let us revive it!"</i></p>

    <h3>Our Services:</h3>
    <ul>
      <li>Screen Replacement — <span class="price">P.1200</span></li><br>
      <img src="https://ph.pinterest.com/pin/314759461478010942/">
      
      
      <li>Battery Installation — <span class="price">P.1500</span></li><br>
      <img src=https://ph.pinterest.com/pin/47710077298947113/">
      
      
    </ul>

    <p>Call us: <a href="tel:5551234">555-1234</a></p>
    
    <button onclick="location.reload()" style="width: auto; padding: 10px 20px;">Back to Home</button>
  </div>

  <script>
    function showServices() {
      document.getElementById("registration-section").style.display = "none";
      document.getElementById("services-section").style.display = "block";
    }
  </script>

</body>
</html>
