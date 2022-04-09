<script lang="ts">
	import { page } from '$app/stores';

	let navActive = false;
</script>

<nav class={`navbar is-fixed-top ` + (navActive ? "is-active":"")} role="navigation" aria-label="main navigation" style="margin-bottom: height;">
<div class="navbar-brand">
	<a class="navbar-item" href="https://bulma.io">
	<img src="https://bulma.io/images/bulma-logo.png" width="112" height="28">
	</a>
	<a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" on:click = {() => {navActive = !navActive}}>
		<span aria-hidden="true"></span>
		<span aria-hidden="true"></span>
		<span aria-hidden="true"></span>
	</a>
</div>

<div class={"navbar-menu " + (navActive ? "is-active":"")}>
	<div class="navbar-start">
	<a class="navbar-item" sveltekit:prefetch href="/">
		Home
	</a>

	<div class="navbar-item has-dropdown is-hoverable">
		<a class="navbar-link" sveltekit:prefetch href="/about">
			About CISCA
		</a>

		<div class="navbar-dropdown">
			<a class="navbar-item" sveltekit:prefetch href="/about">
				About
			</a>
			<a class="navbar-item" sveltekit:prefetch href="/about#values">
				Values
			</a>
			<hr class="navbar-divider">
			<a class="navbar-item" sveltekit:prefetch href="/about#faq">
				FAQ
			</a>
		</div>
	</div>

	<a class="navbar-item" sveltekit:prefetch href="/festival">
		Festival
	</a>
	<a class="navbar-item" sveltekit:prefetch href="/news">
		News
	</a>

	<a class="navbar-item" sveltekit:prefetch href="/contact">
		Contact
	</a>
	</div>

	<div class="navbar-end">
		<div class="navbar-item">
			<div class="buttons">
			<a class="button is-primary" sveltekit:prefetch href="/donate">
				<strong>Donate</strong>
			</a>
			</div>
		</div>
	</div>
</div>
</nav>

<style>

</style>
