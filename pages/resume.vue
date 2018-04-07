<template>
	<section class="container">
		<global-header/>
		THis is where resume would go
	</section>
</template>

<script>
	import AppLogo from '~/components/AppLogo.vue';
	import GlobalHeader from '~/components/GlobalHeader.vue';

	export default {
		components: {
			AppLogo, GlobalHeader
		},
		head () {
			return {
				title: this.title,
				meta: [
					{ hid: 'description', name: 'description', content: 'Front end evanelist and an avid gamer, I build experiences for Web and mobile.' }
				]
			}
		}
	}
</script>

<style>
	.container {
		
	}

	.title {
		font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
		display: block;
		font-weight: 300;
		font-size: 100px;
		color: #35495e;
		letter-spacing: 1px;
	}

	.subtitle {
		font-weight: 300;
		font-size: 42px;
		color: #526488;
		word-spacing: 5px;
		padding-bottom: 15px;
	}

	.links {
		padding-top: 15px;
	}
</style>
