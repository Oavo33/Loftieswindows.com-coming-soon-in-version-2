<html lang="en"><head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Lofties Windows</title>
	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&display=swap">
	<style>@media only screen and (max-width: 600px){header{font-family: "UnifrakturMaguntia";
			background-image: url("https://images.unsplash.com/photo-1534447677768-be436bb09401?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80");
		}.triangle-container 
		.triangle 
	nav 
		nav ul
			nav li 
			nav li
		nav li
		nav li
		nav img
		nav li
    .tab-menu li 
.tab-menu li
.tab-menu li 
.tab-hover .tab-menu li
.tab-menu li
.tab-menu li
.tab-menu li img
h1
h1 span 
h1 span:hover
#typewriter-text 
@keyframes typing {
			from {
				width: 0;
			}
			to {
				width: 100%;
			}
		}@keyframes blink-caret {
			from, to {
				border-color: transparent;
			}
			50% {
				border-color: #333;
			}
		}@keyframes fade-in-out {
			0% {
				opacity: 0;
			}
			50% {
				opacity: 1;
			}
			100% {
				opacity: 0;}
		}@keyframes zoomIn {
			from {
				transform: scale(0.1);
				opacity: 0;
			}
			to {
				transform: scale(1);
				opacity: 1;
			}
		}</style>
<script>
		window.addEventListener('load', () => {
			const canvas = document.getElementById('canvas');
			const context = canvas.getContext('2d');
			canvas.width = window.innerWidth;
			canvas.height = 100;
			const numOfTriangles = 14;
			const triangleWidth = canvas.width / numOfTriangles;
			const triangleHeight = Math.sqrt(0.2) / 2 * triangleWidth;
			const triangleColors = ['#FF0000', '#FF8000', '#FFFF00', '#80FF00', '#00FF00', '#00FF80', '#00FFFF', '#0080FF', '#0000FF', '#8000FF', '#FF00FF', '#FF0080', '#FFFFFF', '#000000'];
			const length = Math.min(numOfTriangles, triangleColors.length);
			for (let i = 0; i < length; i++) {
				context.beginPath();
				context.moveTo(i * triangleWidth, 0);
				context.lineTo((i + 0.414) * triangleWidth, triangleHeight);
				context.lineTo((i + 1) * triangleWidth, 0);
				context.closePath();
				context.fillStyle = triangleColors[i];
				context.fill();
			}
		});
	</script></head>
<body>
	<header>
		<div class="triangle-container">
			<canvas id="canvas"></canvas>
		</div>
		<h1><span>L</span><span>o</span><span>f</span><span>t</span><span>i</span><span>e</span><span>s</span><span>W</span><span>i</span><span>n</span><span>d</span><span>o</span><span>w</span><span>S</span></h1>
		<nav>
			<ul>
				<li><a href="#"><img src="https://img.icons8.com/clouds/32/000000/facebook.png" alt="Facebook"></a></li>
				<li><a href="#"><img src="https://img.icons8.com/clouds/32/000000/discord-logo.png" alt="Discord"></a></li>
				<li><a href="#"><img src="https://img.icons8.com/clouds/64/000000/youtube.png" alt="YouTube"></a></li>
			</ul>
		</nav>
	<ul class="tab-menu">
		<li>
			<img src="https://img.icons8.com/color/48/000000/controller.png" alt="Games">
			Games
			<div class="tab-hover">Why did the sun go to school? To get brighter!</div>
		</li>
		<li>
			<img src="https://img.icons8.com/color/48/000000/youtube-play.png" alt="Videos">
			Videos
			<div class="tab-hover">Why did the astronaut break up with his girlfriend? Because he needed his space!</div>
        </li>
        <li>
          <img src="https://img.icons8.com/color/48/000000/music.png" alt="Music">
          Music
          <div class="tab-hover">Why did the space cookie go to the doctor? Because it felt crummy!</div>
        </li>
    </ul><p id="typewriter-text"></p>
</header>
	<script>@media only screen and (max-width: 600px) {
		const text = "Attention all window lovers! Search our website for the squeegee and win a free clean!";
		let i = 0;
		function typeWriter() {
			if (i < text.length) {
				document.getElementById("typewriter-text").innerHTML += text.charAt(i);
				i++;
				setTimeout(typeWriter, Math.floor(Math.random() * 200) + 50); // randomize the typing speed
			}
		}
		typeWriter();}
	</script>
</body></html>
