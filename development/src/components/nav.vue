<template>
	<nav id="nav">
		<div class="nav-wrapper">
			<div class="mini-nav-container">
				<ul class="nav-social">
					<li><a href="#" class="icon facebook"><span class="label">Facebook</span></a></li>
					<li><a href="#" class="icon twitter"><span class="label">Twitter</span></a></li>
					<li><a href="#" class="icon youtube"><span class="label">Youtube</span></a></li>
				</ul>
				<ul class="nav-utility">
					<li><a href="#">Habitat</a></li>
					<li><a href="#">Helix</a></li>
					<li><a href="#">Sitecore.net</a></li>
				</ul>
			</div>
			<div class="main-nav-container">
				<div class="nav-left">
					<div class="burger">
						MB
					</div>
					<a href="#">
						<!-- Example of next-gen images and fall back code. -->
						<picture>
							<source srcset="../assets/images/logo.webp" type="image/webp">
							<source srcset="../assets/images/logo.jpg" type="image/jpeg">
							<img src="../assets/images/logo.jpg" alt="Habitat Logo">
						</picture>
					</a>
				</div>
				<ul class="nav-center">
					<li><a href="#">Home</a></li>
					<li><a href="#">About Habitat</a></li>
					<li><a href="#">Modules</a></li>
					<li><a href="#">More Info</a></li>
				</ul>
				<div class="nav-right">
					<ul>
						<li><a href="#">Globe</a></li>
						<li><a href="#">Account</a></li>
						<li><a href="#">Search</a></li>
					</ul>
				</div>
			</div>
		</div>
	</nav>
</template>

<script>
export default {
	components: {
	}
}
</script>

<style scoped lang="scss">
	@import '../assets/scss/_variables.scss';
	@import '../assets/scss/_core.scss';
	@import '../assets/scss/_nav.scss';
</style>
