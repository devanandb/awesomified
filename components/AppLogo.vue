<template>
	<div class="VueToNuxtLogo">
		<div class="Triangle Triangle--two"/>
		<div class="Triangle Triangle--one"/>
		<div class="Triangle Triangle--three"/>
		<div class="Triangle Triangle--four"/>
		<div class="Triangle Triangle--five"/>
	</div>
</template>

<style>
	.VueToNuxtLogo {
		display: inline-block;
		animation: turn 2s linear forwards 1s;
		/*transform: rotateX(180deg);*/
		position: relative;
		overflow: hidden;
		height: 180px;
		width: 245px;
	}

	.Triangle {
		position: absolute;
		top: 0;
		left: 0;
		width: 0;
		height: 0;
	}

	.Triangle--one {
		border-left: 105px solid transparent;
		border-right: 105px solid transparent;
		border-bottom: 180px solid #41B883;
		animation: form 0.5s linear forwards 3.5s;

	}

	.Triangle--two {
		top: 30px;
		left: 35px;
		animation: goright 0.5s linear forwards 3.5s;
		border-left: 87.5px solid transparent;
		border-right: 87.5px solid transparent;
		border-bottom: 150px solid #3B8070;
	}

	.Triangle--three {
		top: 60px;
		left: 35px;
		animation: goleft 0.5s linear forwards 3.5s;
		border-left: 70px solid transparent;
		border-right: 70px solid transparent;
		border-bottom: 120px solid #35495E;
	}

	.Triangle--four {
			top: -120px;
			left: 105px;
			-webkit-animation: godown 0.5s linear forwards 3s;
			animation: godown 0.5s linear forwards 3s;
			/* border-left: 20px solid transparent; */
			/* border-right: 20px solid transparent; */
			/* border-bottom: 40px solid #fff; */
			width: 15px;
			height: 108px;
			background-color: #fff;
	}

	.Triangle--five {
		top: 120px;
		left: 100px;
		animation: godown 0.5s linear forwards 3s;
		border-left: 20px solid transparent;
		border-right: 20px solid transparent;
		border-bottom: 40px solid #fff;
		display: none;
	}

	@keyframes turn {
		100% {
			transform: rotateX(0deg);
		}
	}

	@keyframes form {
		100% {
			border-right: 0px solid transparent;
		}
	}
	@keyframes godown {
		100% {
			top: 50px;
		}
	}

	@keyframes goright {
		100% {
			left: 120px;
			border-left: 0px solid transparent;
		}
	}

	@keyframes goleft {
		100% {
			left: 42px;
		}
	}
</style>
