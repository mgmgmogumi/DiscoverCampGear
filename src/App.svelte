<script>
	export let url = "";
	import { Router, Link, Route } from "svelte-routing";
	import Header from './components/Header.svelte';
	import Footer from './components/Footer.svelte';
	import Home from './components/Home.svelte';
	import Create from './components/Create.svelte';
	import Diary from './components/Diary.svelte';
	import About from './components/About.svelte';
</script>

<main>
	<Header />
	<Router url="{url}">
		<Route path="diary/:id" component="{Diary}" />
		<Route path="create" component="{Create}" />
		<Route path="about" component="{About}" />
		<Route path="/"><Home /></Route>
	</Router>
	<div class="footer">
		<Footer/>
	</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	.footer {
		position: absolute;
		bottom: 0;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>