- 👋 Hi, I’m @Suvenduojha
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Suvenduojha/Suvenduojha is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>College Website</title>
	<link rel="stylesheet" href="styles.css">
</head>
<body>
	<header>
		<nav>
			<ul>
				<li><a href="#home">Home</a></li>
				<li><a href="#about">About</a></li>
				<li><a href="#admissions">Admissions</a></li>
				<li><a href="#academics">Academics</a></li>
				<li><a href="#contact">Contact</a></li>
			</ul>
		</nav>
	</header>
	<main>
		<section id="home">
			<h1>Welcome to Our College</h1>
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
		</section>
		<section id="about">
			<h2>About Us</h2>
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
		</section>
		<section id="admissions">
			<h2>Admissions</h2>
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
		</section>
		<section id="academics">
			<h2>Academics</h2>
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
		</section>
		<section id="contact">
			<h2>Contact Us</h2>
			<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
		</section>
	</main>
	<footer>
		<p>&copy; 2023 College Website</p>
	</footer>
	<script src="script.js"></script>
</body>
</html>
```
CSS (styles.css):
```
body {
	font-family: Arial, sans-serif;
	margin: 0;
	padding: 0;
}
header {
	background-color: #333;
	color: #fff;
	padding: 1em;
	text-align: center;
}
nav ul {
	list-style: none;
	margin: 0;
	padding: 0;
	display: flex;
	justify-content: space-between;
}
nav li {
	margin-right: 20px;
}
nav a {
	color: #fff;
	text-decoration: none;
}
main {
	display: flex;
	flex-direction: column;
	align-items: center;
	padding: 2em;
}
section {
	background-color: #f7f7f7;
	padding: 2em;
	margin-bottom: 20px;
	box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
h1, h2 {
	color: #333;
}
footer {
	background-color: #333;
	color: #fff;
	padding: 1em;
	text-align: center;
	clear: both;
}
```
JavaScript (script.js):
```
// Add event listener to navigation menu
document.querySelector('nav').addEventListener('click', function(event) {
	if (event.target.tagName === 'A') {
		event.preventDefault();
		var sectionId = event.target.getAttribute('href').replace('#', '');
		document.querySelector(`#${sectionId}`).scrollIntoView({ behavior: 'smooth' });
	}
});
```
