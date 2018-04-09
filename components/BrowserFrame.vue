<template>
	<div class="browser">
		<div class="title-bar">
			<div class="actions">
				<span></span>
				<span></span>
				<span></span>
			</div>
		</div>
		asdasdasdasd
	</div>
</template>

<style lang="scss">
	.browser {
		width: 100%;
		background-color: #fff;
		min-height: 300px;
		border-top-left-radius: 5px;
		border-top-right-radius: 5px;
		.title-bar {
			background-color: #c1bcbc;
			.actions {
				padding: 12px;
				span {
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
	}
</style>
