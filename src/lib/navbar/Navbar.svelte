<script lang="ts">
	import { page } from '$app/stores';

	let navActive: boolean = false;
</script>

<nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation" style="margin-bottom: height;">
<div class="navbar-brand">
	<div class="navbar-item">
	<img src="/logo.png">
	</div>
	<a role="button" class={"navbar-burger "+ (navActive ? "is-active":"")} aria-label="menu" aria-expanded="false" on:click = {() => {navActive = !navActive}}>
		<span aria-hidden="true"></span>
		<span aria-hidden="true"></span>
		<span aria-hidden="true"></span>
	</a>
</div>

<div class={"navbar-menu " + (navActive ? "is-active":"")}>
	<div class="navbar-start">
	<a class="navbar-item" sveltekit:prefetch href="/"  on:click = {() => {navActive = !navActive}}>
		Home
	</a>

	<div class="navbar-item has-dropdown is-hoverable">
		<a class="navbar-link" sveltekit:prefetch href="/about"  on:click = {() => {navActive = !navActive}}>
			About CICSA
		</a>

		<div class="navbar-dropdown">
			<a class="navbar-item" sveltekit:prefetch href="/about#mission"  on:click = {() => {navActive = !navActive}}>
				Mission
			</a>
			<a class="navbar-item" sveltekit:prefetch href="/about#values"  on:click = {() => {navActive = !navActive}}>
				Values
			</a>
			<hr class="navbar-divider">
			<a class="navbar-item" sveltekit:prefetch href="/about#faq"  on:click = {() => {navActive = !navActive}}>
				FAQ
			</a>
		</div>
	</div>

	<div class="navbar-item has-dropdown is-hoverable" on:click = {() => {navActive = !navActive}}>
		<a class="navbar-link" sveltekit:prefetch href="/festival" on:click = {() => {navActive = !navActive}}>
			Chinese Festival
		</a>
		<div class="navbar-dropdown">
			<a class="navbar-item" sveltekit:prefetch href="/festival/leaders"  on:click = {() => {navActive = !navActive}}>
				Department Leaders
			</a>
		</div>
	</div>
	<a class="navbar-item" sveltekit:prefetch href="/contact"  on:click = {() => {navActive = !navActive}}>
		Contact
	</a>
	</div>

	<div class="navbar-end">
		<div class="navbar-item">
			<div class="buttons">
			<a class="button is-primary" sveltekit:prefetch href="/donate"  on:click = {() => {navActive = !navActive}}>
				<strong>Donate</strong>
			</a>
			</div>
		</div>
	</div>
</div>
</nav>

<style>
</style>
