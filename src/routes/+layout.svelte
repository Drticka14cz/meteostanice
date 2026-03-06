<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>



<main>
<div id="telo">

	<div id="stranka">{@render children()}</div>
	<div id="patka">
	<div id="patka_1"><a id="nadpis_patky">projekt Meteostanice</a></div>
	<div id="patka_2"><div id="patka_text" class="patka_div">
			<ul>
				<li class="bez_odrazky hlavni_sekce "><span class="podtrhnuto">Autoři:</span> <ul><li class="bez_odrazky">Jakub Štěpánek</li>
				<li class="bez_odrazky">Tomáš Tarábek</li></ul></li>
				<li class="bez_odrazky hlavni_sekce"><span class="podtrhnuto">Vedoucí práce:</span> <ul>
					<li class="bez_odrazky">Ing. Lukáš Jacečko</li>
				</ul></li>
				<li class="bez_odrazky hlavni_sekce"> <span class="podtrhnuto">Kontakty</span>
					<ul>
						<li class="bez_odrazky">Jakub Štěpánek: stepanek123@trebesin.cz</li>
						<li class="bez_odrazky">Tomáš Tarábek: tarabek123@trebesin.cz</li>
						<li class="bez_odrazky">Ing. Lukáš Jacečko: jacecko@trebesin.cz</li>
					</ul>
				</li>
			</ul>
			
		</div>
		<div id="patka_logo" class="patka_div"><img src="trebesin_logo.png" alt="Logo Třebešín" id="logo_trebesin"></div>
</div>
	<div id="patka_3">2026</div>
		
	</div>



</div>


</main>
<style>
	@import url('https://fonts.googleapis.com/css2?family=Source+Code+Pro:ital,wght@0,200..900;1,200..900&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&family=Source+Code+Pro:ital,wght@0,200..900;1,200..900&display=swap');


	:root {
  --font-base: 'Source Code Pro', monospace;
  --font-mono: 'Source Code Pro', monospace;
}
	#telo{
		width: 100vw;
		max-width: 100%;
		min-height: 100vh;
		/* width: 100%;
		box-sizing: border-box;
		padding: 20px; */
		background-color: rgb(228, 228, 228);
		display: flow-root;
	}
	
	:global(body){
		background-color: aqua;
		padding: 0px;
		margin: 0px;
		font-size: 16px;
		font-family: var(--font-base);
	}
	#patka{
		width: auto;
		min-height: 25rem;
		background-color:  #06d6a0;
		display: block;
		gap: 10px;
		padding: 10px 25px 10px 25px;
		
		
	}
	#patka_text{
		
		/* border: 1px black solid; */
		padding-left: 7%;
		color: black;
		font-family: var(--font-base);
		font-size: medium;
		
	}
	#patka_logo{
		/* border: 1px black solid; */
		display: flex;
		flex-direction: column;
		justify-content: center;
		padding-left: 10rem;

	}
	.patka_div{
		width:100% ;
	}
	.bez_odrazky{
		list-style-type: none;
		font-size: 0.9rem;
		padding-left: 1rem;
	}
	.podtrhnuto{
		text-decoration: underline;
		font-size: 1.2rem;
		
	}
	.hlavni_sekce{
		margin-bottom: 1.5rem;
	}
	#patka_1, #patka_2, #patka_3{
		/* border: 2px dashed red; */
		min-height: 3rem;
	}
	#patka_1, #patka_3{
		text-align: center;
		padding-top: 1%;
		

	}
	#patka_3{
		display: flex;
		flex-direction: column;
		justify-content: flex-end;
	}
	#patka_2{
		display: flex;
	}
	#logo_trebesin{
		max-width: 25rem;
	}
	#nadpis_patky{
		font-family: var(--font-mono);
		font-size: 1.6 rem;
	}
</style>