# Ex.06 Restaurant Website
# Date: 28-05-2026
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
Style.css
```
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background-color: #fff8f0;
  color: #333;
}

header {
  background-color: #c0392b;
  color: white;
  padding: 15px 0;
  text-align: center;
}

nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

nav ul li {
  display: inline;
  margin: 0 15px;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

nav ul li a:hover {
  text-decoration: underline;
}

/* ====== Hero Section ====== */
.hero {
  text-align: center;
  padding: 70px 20px;
  background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
    url('https://images.unsplash.com/photo-1551782450-17144efb9c50');
  background-size: cover;
  background-position: center;
  color: white;
}

.hero h2 {
  font-size: 2.5em;
  margin-bottom: 10px;
}

.hero p {
  font-size: 1.2em;
  margin-bottom: 20px;
}

.btn {
  background-color: #e67e22;
  color: white;
  padding: 10px 20px;
  text-decoration: none;
  border-radius: 5px;
}

.btn:hover {
  background-color: #d35400;
}

/* ====== Menu Section ====== */
.menu {
  padding: 30px;
  text-align: center;
}

.menu-item {
  background: #ffe6e6;
  margin: 15px auto;
  padding: 15px;
  width: 60%;
  border-radius: 10px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
}

/* ====== Gallery Section ====== */
.gallery {
  padding: 30px;
  text-align: center;
}

.gallery h2 {
  margin-bottom: 20px;
  color: #c0392b;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 15px;
  margin: 0 auto;
  max-width: 1000px;
}

.gallery-grid img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  border-radius: 10px;
  transition: transform 0.3s, box-shadow 0.3s;
}

.gallery-grid img:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
}

/* ====== About Section ====== */
.about {
  padding: 30px;
  text-align: center;
  width: 80%;
  margin: auto;
}

/* ====== Contact Section ====== */
.contact {
  padding: 30px;
  text-align: center;
}

.reservation-form {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 60%;
  margin: 20px auto;
}

.reservation-form input,
.reservation-form textarea {
  width: 100%;
  padding: 10px;
  margin: 8px 0;
  border-radius: 5px;
  border: 1px solid #ccc;
}

.reservation-form button {
  background-color: #c0392b;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
}

.reservation-form button:hover {
  background-color: #a93226;
}

/* ====== Footer ====== */
footer {
  background-color: #c0392b;
  color: white;
  text-align: center;
  padding: 10px;
  position: relative;
  bottom: 0;
  width: 100%;
}
```
About.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About - Abhinava Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>About Us</h1>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="menu.html">Menu</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="about">
    <h2>Welcome to Abhinava Restaurant</h2>
    <p>Abhinava Family Restaurant is a popular dining spot located in Ramnagar, Anantapur, known for its extensive menu and cozy ambiance. It offers a mix of North Indian, South Indian, and Chinese cuisines, with specialties like their Tandoori Biryani, Chicken Sizzler, and Special Chicken Biryani.</p>

    <p>From Indian classics to continental delights, we believe every plate tells a story. 
    Come, experience food made with love and served with warmth.  It is a 4.5-star rated establishment across platforms like Justdial. Patrons report both enjoyable dining experiences and notable service inconsistencies.</p>
  </section>

  <footer>
    <p>© 2026 Abhinava Restaurant</p>
  </footer>
</body>
</html>
```
Index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Abhinava Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Abhinava Restaurant</h1>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="menu.html">Menu</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <h2>Delicious Food, Cozy Ambience</h2>
    <p>Experience the best dishes made with love and fresh ingredients.</p>
    <a href="menu.html" class="btn">Explore Menu</a>
  </section>

  <footer>
    <p>© 2026 Abhinava Restaurant | Designed by Harsha Reddy</p>
  </footer>
</body>
</html>
```
Menu.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Menu - Abhinava Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Our Menu</h1>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="menu.html">Menu</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="menu">
    <div class="menu-item">
      <h3>Grilled Chicken</h3>
      <p>Served with garlic sauce and fries — ₹250</p>
    </div>
    <div class="menu-item">
      <h3>Paneer Butter Masala</h3>
      <p>Creamy tomato-based curry with soft paneer cubes — ₹200</p>
    </div>
    <div class="menu-item">
      <h3> Chicken Biriyani</h3>
      <p>Spicy and flavorful rice loaded with veggies & chicken — ₹300</p>
    </div>
    <div class="menu-item">
      <h3>Chocolate Lava Cake</h3>
      <p>Cool chocolate delight — ₹180</p>
    </div>
  </section>

  <footer>
    <p>© 2026 Abhinava Restaurant</p>
  </footer>
</body>
</html>
```
Gallery.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gallery - Abhinava Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Our Gallery</h1>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="menu.html">Menu</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="gallery">
    <h2>Delicious Moments Captured</h2>
    <div class="gallery-grid">
      <img src="biryani.jpg" alt="Chicken Biriyani">
      <img src="salad.jpg" alt="Fresh Salad">
      <img src="pizza.jpg" alt="Pizza">
      <img src="cake.jpeg" alt="Dessert">
      <img src="dosa.jpg" alt="Dosa">
      <img src="cool drink.jpg" alt="Cool Drink">    </div>
  </section>

  <footer>
    <p>© 2026 Abhinava Restaurant</p>
  </footer>
</body>
</html>
```
Contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact - Abhinava Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Contact Us</h1>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="menu.html">Menu</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="contact">
    <h2>Get in Touch</h2>
    <p>📍 Location: Opp to 80 Feet Road, Ram Nagar, Anantapur, Andhra Pradesh, 515004</p>
    <p>📞 Phone: +91 85542 24004</p>
    <p>✉️ Email: hello@abhinavarestaurant.com</p>

    <h3>Reserve a Table</h3>
    <form class="reservation-form">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Email Address" required>
      <input type="tel" placeholder="Phone Number" required>
      <input type="date" required>
      <input type="time" required>
      <textarea placeholder="Special Requests"></textarea>
      <button type="submit">Book Now</button>
    </form>
  </section>

  <footer>
    <p>© 2026 Abhinava Restaurant</p>
  </footer>
</body>
</html>
```

# OUTPUT:
<img width="1907" height="693" alt="home" src="https://github.com/user-attachments/assets/114eb720-6b20-4679-a4b8-2ab0ddff3bb8" />

<img width="1918" height="637" alt="about" src="https://github.com/user-attachments/assets/de62cc67-6e49-40a6-90ca-1663b36f8c93" />

<img width="1913" height="992" alt="menu" src="https://github.com/user-attachments/assets/8cc8d6a9-91b0-4466-9f2a-5a51d804f31c" />

<img width="1917" height="1008" alt="gallery" src="https://github.com/user-attachments/assets/217bccc5-78f7-4eb5-b989-a16cca4e43d3" />

<img width="1918" height="1064" alt="contact" src="https://github.com/user-attachments/assets/35e342ee-53f4-444f-a767-06d97f311bf2" />

# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
