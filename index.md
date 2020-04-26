Skip to content
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 
@mikebuono 
Learn Git and GitHub without any code!
Using the Hello World guide, you’ll start a branch, write comments, and open a pull request.


flexdinesh
/
dev-landing-page
Template
26
848447
 Code Issues 0 Pull requests 1 Actions Projects 0 Wiki Security 0 Insights
Dev Landing Page with 9 themes : )

 master
@flexdinesh
flexdinesh committed on Mar 8, 2018 
1 parent 11923e3 commit a70146ec429f773b399cf704730f1eb1caa6b93f
Showing  with 265 additions and 0 deletions.
 25  css/reset.css 
@@ -0,0 +1,25 @@
/* Minimal CSS Reset */

html {
  box-sizing: border-box;
  font-size: 12px;
}

*, *:before, *:after {
  box-sizing: inherit;
}

body, h1, h2, h3, h4, h5, h6, p, ol, ul {
  margin: 0;
  padding: 0;
  font-weight: normal;
}

ol, ul {
  list-style: none;
}

img {
  max-width: 100%;
  height: auto;
} 
 71  css/styles.css 
@@ -0,0 +1,71 @@
/* Typography */

html {
	font-family: 'Roboto', sans-serif;
}

@media (min-width: 576px) {
	html {
		font-size: 14px;
	}
}

@media (min-width: 768px) {
	html {
		font-size: 16px;
	}
}

@media (min-width: 992px) {
	html {
		font-size: 18px;
	}
}

@media (min-width: 1200px) {
	html {
		font-size: 20px;
	}
}

.icons-social i {
	font-size: 3em;
}

/* Custom Styles */

main {
	display: flex;
	flex-direction: column;
	min-height: 100vh;
	justify-content: center;
	padding: 0 30px;
	text-align: center;
}

main > .intro {
	font-family: 'Reem Kufi', sans-serif;
	font-size: 3.75em;
	font-weight: 600;
}

main > .tagline {
	font-size: 1.5rem;
	margin: 1.5rem 0;
	font-weight: 100;
}

.icons-social i {
	padding: 10px;
}

.devto {
	margin-bottom: -0.20rem;
}

.devto svg {
	margin-bottom: -0.20rem;
	margin-left: 0.675rem;;
	width: 2.65rem;
	height: 2.65rem;
} 
 14  css/themes/green-white.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #43A047;
	color: #FAFAFA;
}

.icons-social a {
	color: #FAFAFA;
}

.icons-social a svg path{
	fill: #FAFAFA;
} 
 14  css/themes/grey-white.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #485564;
	color: #FAFAFA;
}

.icons-social a {
	color: #FAFAFA;
}

.icons-social a svg path{
	fill: #FAFAFA;
} 
 14  css/themes/indigo-white.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #303F9F;
	color: #FAFAFA;
}

.icons-social a {
	color: #FAFAFA;
}

.icons-social a svg path{
	fill: #FAFAFA;
} 
 14  css/themes/red-white.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #AF3D4E;
	color: #FAFAFA;
}

.icons-social a {
	color: #FAFAFA;
}

.icons-social a svg path{
	fill: #FAFAFA;
} 
 14  css/themes/white-blue.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #FAFAFA;
	color: #0277BD;
}

.icons-social a {
	color: #0277BD;
}

.icons-social a svg path{
	fill: #0277BD;
} 
 14  css/themes/white-grey.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #EDEDED;
	color: #4B5658;
}

.icons-social a {
	color: #4B5658;
}

.icons-social a svg path{
	fill: #4B5658;
} 
 14  css/themes/white-indigo.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #E8EAF6;
	color: #303F9F;
}

.icons-social a {
	color: #303F9F;
}

.icons-social a svg path{
	fill: #303F9F;
} 
 14  css/themes/white-red.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #EDEDED;
	color: #AF3D4E;
}

.icons-social a {
	color: #AF3D4E;
}

.icons-social a svg path{
	fill: #AF3D4E;
} 
 14  css/themes/yellow-black.css 
@@ -0,0 +1,14 @@
/* Theme */

main {
	background: #FFEB3B;
	color: #1E1E1E;
}

.icons-social a {
	color: #1E1E1E;
}

.icons-social a svg path{
	fill: #1E1E1E;
} 
 BIN +5.43 KB favicon.ico 
Binary file not shown.
 43  index.html 
@@ -0,0 +1,43 @@
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">

	<title>Dinesh Pandiyan | Awesome Dev</title>

	<link rel="shortcut icon" href="favicon.ico" type="image/x-icon" />

	<link href="https://fonts.googleapis.com/css?family=Reem+Kufi|Roboto:300" rel="stylesheet">
	<link href="https://use.fontawesome.com/releases/v5.0.8/css/all.css" rel="stylesheet">
	<link rel="stylesheet" href="css/reset.css">
	<link rel="stylesheet" href="css/styles.css">
	<link rel="stylesheet" href="css/themes/indigo-white.css">
	<!-- <link rel="stylesheet" href="css/themes/green-white.css"> -->
	<!-- <link rel="stylesheet" href="css/themes/red-white.css"> -->
	<!-- <link rel="stylesheet" href="css/themes/grey-white.css"> -->
	<!-- <link rel="stylesheet" href="css/themes/white-indigo.css"> -->
	<!-- <link rel="stylesheet" href="css/themes/white-blue.css"> -->
	<!-- <link rel="stylesheet" href="css/themes/white-grey.css"> -->
	<!-- <link rel="stylesheet" href="css/themes/white-red.css"> -->
	<!-- <link rel="stylesheet" href="css/themes/yellow-black.css"> -->
</head>
<body>
	<main>
		<div class="intro">Hello, I'm Dinesh!</div>
		<div class="tagline">All-Star Dev | Code Fanatic | Linux Hacker | Bleh</div>
		<!-- Find your icons from here - https://fontawesome.com/icons?d=gallery&s=brands -->
		<div class="icons-social">
			<a target="_blank" href="https://github.com/flexdinesh"><i class="fab fa-github"></i></a>
			<a target="_blank" href="https://twitter.com/flexdinesh"><i class="fab fa-twitter"></i></a>
			<a target="_blank" href="https://stackoverflow.com/story/flexdinesh"><i class="fab fa-stack-overflow"></i></a>
			<a target="_blank" href="https://www.linkedin.com/in/dineshpandiyan"><i class="fab fa-linkedin"></i></a>
			<a target="_blank" href="https://medium.com/@flexdinesh"><i class="fab fa-medium"></i></a>
			<a target="_blank" href="https://www.freecodecamp.org"><i class="fab fa-free-code-camp"></i></a>
			<a target="_blank" href="https://www.behance.net"><i class="fab fa-behance"></i></a>
			<a target="_blank" href="https://codepen.io"><i class="fab fa-codepen"></i></a>
    </div>
	</main>
</body>
</html> 
0 comments on commit a70146e
@mikebuono
 
 
Leave a comment

Attach files by dragging & dropping, selecting or pasting them.
 You’re not receiving notifications from this thread.
© 2020 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About

