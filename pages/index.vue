<template>
	<div class="container">
		<global-header/>
			<!-- <app-logo/> -->
			
		<section class="hero">
			<div class="txt-blk">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quam, cupiditate.</div>
			<div class="img-blk">
				<div class="browser-fr">
					<browser-frame></browser-frame>
				</div>
			</div>
		</section>
	</div>
</template>

<script>
	import AppLogo from '~/components/AppLogo.vue';
	import GlobalHeader from '~/components/GlobalHeader.vue';
	import BrowserFrame from '~/components/BrowserFrame.vue';

	export default {
		components: {
			AppLogo, GlobalHeader, BrowserFrame
		},
		head () {
			return {
				title: 'Home | Devanand Babu portfolio & webconnect',
				meta: [
					{ hid: 'description', name: 'description', content: 'I enjoy turning complex problems into simple, tangible and intuitive solutions. When I\'m not coding, tweeting or pushing pixels, you\'ll find me gaming, eating or exercising in the park(lie).' }
				]
			}
		}
	}
</script>

<style>
	body {
		background-image: linear-gradient(-45deg, #9B42DA 0%, #51509C 62%);
		color: #fff;
		margin: 0px;
		padding: 0px;
	}
	.container {
		min-height: 100vh;
		width: 1200px;
		margin: auto;
		
	}

	.hero {
		vertical-align: middle;
		margin-top: 40px;
	}
	.hero .txt-blk {
		font-family: Helvetica;
		font-size: 28px;
		color: #FFFFFF;
		letter-spacing: 0;
		text-align: left;
		line-height: 47px;
		width: 500px;
		display: inline-block;
		/*margin-top: 200px;*/
		vertical-align: middle;
		margin-right: 50px;
	}
	.hero .img-blk {
		display: inline-block;
		vertical-align: middle;
	}
	
	.browser-fr {
		width: 600px;
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
