<script>
	import "../app.pcss";
	import Experience from "./components/Experience/Experience.svelte";
    import Header from './components/Header.svelte';
	import Profile from "./components/Profile.svelte";
    import './styles.css';
</script>

<div class="app">
	<Header/>
	<Profile/>
	<Experience/>

	<main>
		<slot></slot>
	</main>
</div>

