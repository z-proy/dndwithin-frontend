<script lang="ts">
	import { Button, Form, Input } from 'spaper'
	import Logincard from '../lib/Logincard.svelte'
</script>

<main>
	<link rel="stylesheet" href="https://unpkg.com/papercss@1.8.3/dist/paper.min.css">
	<div class="loginGrid"><Logincard /></div>
</main>

<style>
	main {
		display: grid;
		place-items: center;
	}

	@media (min-width: 600px) {
		main {
			max-width: none;
		}
		h1 {
			color: blueviolet;
		}
	}
</style>