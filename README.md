<!DOCTYPE html>
<html lang="en">

<head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<link rel="stylesheet" href="/css/style.css">
	<title>Meditation App</title>
</head>

<body>

	<div class="app">
		<!--  Контейнер видео бэкграунд  -->
		<div class="video-container">
			<!--  повторяет видео с начала после его зацикливания -->
			<video loop>
				<source src="/video/mountain.mp4" type="video/mp4">
			</video>
		</div>
		<!-- Класс выбора времени -->
		<div class="time-select">
			<!-- The data-* собственный атрибут, добавляет дополнительные данные к элементу -->
			<button data-time="120">2 Minutes</button>
			<button data-time="300">5 Minutes</button>
			<button data-time="600">10 Minutes</button>
			<button data-time="1200">20 Minutes</button>
		</div>

		<!-- Класс PLAY/PAUSE Бэкграунда И ТАЙМЕР -->
		<div class="player-contayner">
			<audio class="song">
				<source src="/sounds/Ma4u-Pik4u.mp3">
			</audio>
			<img src="/svg/play.svg" alt="play" class="play">
			<!-- outline - белый контур -->
			<svg class="track-outline" width="453" height="453" viewBox="0 0 453 453" fill="none"
				xmlns="http://www.w3.org/2000/svg">
				<circle cx="226.5" cy="226.5" r="216.5" stroke="white" stroke-width="20" />
			</svg>
			<!-- outline - синий контур -->
			<svg class="moving-outline" width="453" height="453" viewBox="0 0 453 453" fill="none"
				xmlns="http://www.w3.org/2000/svg">
				<circle cx="226.5" cy="226.5" r="216.5" stroke="#018EBA" stroke-width="20" />
			</svg>
			<!-- Показывает таймер обратного отсчета -->
			<h3 class="time-display">0:00</h3>
		</div>
		<!-- Класс музыки и видео -->
		<div class="sound-picker">
			<!-- The data-* атрибут добавляет дополнительные данные к элементу -->
			<button data-sound="/sounds/rain.mp3" data-video="/video/дождь.mp4">
				<img src="/svg/rain.svg" alt="rain">
			</button>
			<button data-sound="/sounds/beach.mp3" data-video="/video/sea.mp4">
				<img src="/svg/beach.svg" alt="beach">
			</button>
		</div>
	</div>
	<script src="/script/script.js"></script>
</body>

</html>
