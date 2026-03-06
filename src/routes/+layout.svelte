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
	<div id="patka_1">projekt Meteostanice</div>
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
	
	#telo{
		width: 100vw;
		max-width: 100%;
		min-height: 100vh;
		/* width: 100%;
		box-sizing: border-box;
		padding: 20px; */
		background-color: rgb(191, 191, 191);
		display: flow-root;
	}
	
	:global(body){
		background-color: aqua;
		padding: 0px;
		margin: 0px;
	}
	#patka{
		width: auto;
		min-height: 25rem;
		background-color: #1d71b8;
		display: block;
		gap: 10px;
		padding: 10px 25px 10px 25px;
		
		
	}
	#patka_text{
		font-size: large;
		/* border: 1px black solid; */
		padding-left: 10%;
		
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
		font-size: large;
		padding-left: 1rem;
	}
	.podtrhnuto{
		text-decoration: underline;
		
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
</style>