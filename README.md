<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Pizza Glory Reservation</title>
  <link rel="stylesheet" href="style.css"/>
  * {
  box-sizing: border-box;
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

body {
  background: #fff;
  color: #333;
}

header {
  background: url('pizza-bg.jpg') center/cover no-repeat;
  text-align: center;
  color: white;
  padding-bottom: 2rem;
}

.top-nav {
  display: flex;
  justify-content: space-between;
  padding: 1rem 2rem;
  align-items: center;
  background-color: rgba(0, 0, 0, 0.6);
}

.logo {
  height: 50px;
}

nav a {
  color: white;
  margin: 0 1rem;
  text-decoration: none;
}

.book-btn {
  background-color: white;
  color: black;
  padding: 0.5rem 1rem;
  border: none;
  cursor: pointer;
  font-weight: bold;
}

.hero h1 {
  font-size: 2.5rem;
  margin-top: 3rem;
  letter-spacing: 2px;
}

.reservation {
  max-width: 800px;
  margin: 2rem auto;
  padding: 1rem;
  text-align: center;
}

.reservation h2 {
  font-size: 1.8rem;
  margin-bottom: 0.5rem;
}

.reservation p {
  margin-bottom: 1.5rem;
  color: #666;
}

form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.form-group {
  display: flex;
  gap: 1rem;
}

input, select, textarea {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

textarea {
  min-height: 100px;
  resize: vertical;
}

.submit-btn {
  background-color: #222;
  color: white;
  border: none;
  padding: 0.75rem;
  font-weight: bold;
  border-radius: 5px;
  cursor: pointer;
  width: 200px;
  margin: 0 auto;
}

footer {
  margin-top: 3rem;
  text-align: center;
}

.footer-logo {
  height: 60px;
  margin: 1rem auto;
}

</head>
<body>
  <header>
    <div class="top-nav">
      <img src="logo.png" alt="Pizza Glory Logo" class="logo" />
      <nav>
        <a href="#">HOME</a>
        <a href="#">MENU</a>
        <a href="#">CONTACT</a>
        <button class="book-btn">BOOK A TABLE</button>
      </nav>
    </div>
    <div class="hero">
      <h1>PIZZAGLORY <br />RESERVATION</h1>
    </div>
  </header>

  <main>
    <section class="reservation">
      <h2>RESERVE A TABLE</h2>
      <p>CALL US +1700 0363 OR COMPLETE THE FORM BELOW</p>

      <form id="reservationForm">
        <div class="form-group">
          <input type="text" id="name" placeholder="Full Name" required />
          <input type="tel" id="phone" placeholder="Mobile" required />
        </div>
        <div class="form-group">
          <input type="email" id="email" placeholder="Enter Email Address" required />
          <input type="date" id="date" required />
        </div>
        <div class="form-group">
          <input type="time" id="startTime" required />
          <input type="time" id="endTime" required />
        </div>
        <div class="form-group">
          <select id="tableType" required>
            <option value="">Select Table Type</option>
            <option value="birthday">Birthday</option>
            <option value="anniversary">Anniversary</option>
            <option value="casual">Casual</option>
          </select>
          <input type="text" id="guest" placeholder="Guest Full Name" required />
        </div>
        <textarea id="description" placeholder="Type Here..." maxlength="1000"></textarea>
        <button type="submit" class="submit-btn">BOOK A TABLE</button>
      </form>
    </section>
  </main>

  <footer>
    <img src="logo.png" alt="Pizza Glory Footer Logo" class="footer-logo" />
  </footer>

  <script src="script.js"></script>
</body>
</html>
