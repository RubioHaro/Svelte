<script>
	import About from "./components/About.svelte"
	export let name;
	export let lastname;
	let sveltLogo = "https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/b69dbfb1-10d3-457a-848f-bc961f885c10/daj9lav-b42a337a-1d26-4f21-ba88-a74002453c76.png/v1/fill/w_1062,h_752,q_70,strp/the_tale_of_uncle_iroh_by_juggernaut_art_daj9lav-pre.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOiIsImlzcyI6InVybjphcHA6Iiwib2JqIjpbW3siaGVpZ2h0IjoiPD0yMTU1IiwicGF0aCI6IlwvZlwvYjY5ZGJmYjEtMTBkMy00NTdhLTg0OGYtYmM5NjFmODg1YzEwXC9kYWo5bGF2LWI0MmEzMzdhLTFkMjYtNGYyMS1iYTg4LWE3NDAwMjQ1M2M3Ni5wbmciLCJ3aWR0aCI6Ijw9MzA0MyJ9XV0sImF1ZCI6WyJ1cm46c2VydmljZTppbWFnZS5vcGVyYXRpb25zIl19.bXbn1jcMGOsgIGGOzZ63Zle-nhV_tR124qmEe6-kZu4"
</script>

<main>
	<h1>Hello {name} {lastname} !</h1>
	<h3>"La perfeccion y el poder estan sobrevaloreados. Creo, veraderamente que es mas sabio elegir la felicidad y el amor"</h3>
	<About></About>
	<br/>
	<img src={sveltLogo} alt="iroh" />
</main>

<style>

	:global(body){
		background-color: tan;
		color: var(--theme-color);
		
	}

	:global(:root){
		--theme-color: brown
	}

	h3 {
		font-style: italic !important;
		color: var(--theme-color);
		font-size: 30px;
	}

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	main img {
		width: 60%;
	}

	h1 {
		color: white;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>