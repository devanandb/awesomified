<template>
	<div class="browser">
		<div class="title-bar">
			<div class="actions">
				<div></div>
				<div></div>
				<div></div>
			</div>
		</div>
		<div class="window">
			<img src="~/assets/microfocus.jpg" alt="">
		</div>
	</div>
</template>

<style lang="scss">
	.browser {
		width: 100%;
		background-color: #fff;
		min-height: 300px;
		border-radius: 4px;
		box-shadow: 0 36px 43px 0 rgba(0,0,0,0.20);
		.title-bar {
			background-color: #c1bcbc;
			border-top-left-radius: 4px;
			border-top-right-radius: 4px;
			height:30px;
			.actions {
				display:inline-block;
				padding-left: 10px;
				div {
					display:inline-block;
					width: 8px;
					height: 8px;
					border-radius: 50%;
					margin-right: 5px;
					&:first-child {
						background-color: #ff544d;
						border: 1px solid #da3c37;
					}
					&:nth-child(2) {
						background-color: #ffb429;
						border: 1px solid #d99415;
					}
					&:nth-child(3) {
						background-color: #24c238;
						border: 1px solid #119f25;
					}
				}
			}

		}
		.window {
			height: 450px;
			overflow-y: scroll;
			z-index: 10;
			position: relative;
		}
	}
</style>
