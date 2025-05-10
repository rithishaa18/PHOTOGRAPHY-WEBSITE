# PHOTOGRAPHY-WEBSITE
photography-website/
├── index.html
├── about.html
├── contact.html
├── style.css
├── script.js
└── images/
    ├── sample1.jpg
    ├── sample2.jpg
    └── sample3.jpg

1.INDEX.HTNL
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rithisha's Photography</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Rithisha's Photography</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="about.html">About</a>
      <a href="contact.html">Contact</a>
    </nav>
  </header>

  <section class="gallery">
    <h2>My Photo Gallery</h2>
    <div class="photo-slider">
      <div class="slide fade">
        <img src="images/sample1.jpg" alt="Sample 1">
      </div>
      <div class="slide fade">
        <img src="images/sample2.jpg" alt="Sample 2">
      </div>
      <div class="slide fade">
        <img src="images/sample3.jpg" alt="Sample 3">
      </div>
    </div>
  </section>

  <script src="script.js"></script>
</body>
</html>
2.ABOUT.HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Me</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>About Rithisha</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="about.html">About</a>
      <a href="contact.html">Contact</a>
    </nav>
  </header>
  <section>
    <p>I'm Rithisha, passionate about photography and web development. This site showcases some of my favorite photos!</p>
  </section>
</body>
</html>
3.CONTACT.HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Contact Me</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="about.html">About</a>
      <a href="contact.html">Contact</a>
    </nav>
  </header>

  <section>
    <form>
      <label for="name">Name: <input type="text" id="name" required></label><br>
      <label for="email">Email: <input type="email" id="email" required></label><br>
      <label for="message">Message: <textarea id="message" rows="4" required></textarea></label><br>
      <button type="submit">Send</button>
    </form>
  </section>
</body>
</html>
4.STYLES.CSS
/* General styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

header {
  background-color: #333;
  color: white;
  padding: 1rem;
  text-align: center;
}

nav a {
  margin: 0 10px;
  color: white;
  text-decoration: none;
}

nav a:hover {
  text-decoration: underline;
}

/* Gallery styles */
.gallery {
  padding: 1rem;
  text-align: center;
}

.photo-slider {
  position: relative;
  max-width: 1000px;
  margin: auto;
}

.slide {
  display: none;
}

img {
  width: 100%;
  height: auto;
  border-radius: 10px;
}

/* Form styles */
form {
  max-width: 400px;
  margin: auto;
  padding: 1rem;
}

label {
  display: block;
  margin-bottom: 10px;
}

textarea {
  width: 100%;
  resize: vertical;
}

button {
  background-color: #333;
  color: white;
  padding: 10px;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #555;
}
5.SCRIPT.JS
// JavaScript for the photo slider
let slideIndex = 0;
showSlides();

function showSlides() {
  let slides = document.getElementsByClassName("slide");
  for (let i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}    
  slides[slideIndex-1].style.display = "block";  
  setTimeout(showSlides, 3000); // Change image every 3 seconds
}
6. Images:
Create an images folder inside the photography-website folder.

Upload sample1.jpg, sample2.jpg, and sample3.jpg (or use any sample photos you have).

