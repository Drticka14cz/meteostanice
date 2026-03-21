<script>
	import favicon from '/slunce.png';
	// $lib/assets/favicon.svg

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>MeteostanicA</title>
</svelte:head>



<main>
<div id="telo">
	
	<div id="stranka">{@render children()}</div>
	<div id="patka">
	<div id="patka_1"><a id="nadpis_patky">PROJEKT METEOSTANICE</a><div id="patka_odkazy_web"><div class="patka_odkaz_web_divy"><a href="/" class="patka_odkaz_web_divy_a">DOMŮ</a></div>
	<div class="patka_odkaz_web_divy"><a href="/navody" class="patka_odkaz_web_divy_a">NÁVODY</a></div>
	<div class="patka_odkaz_web_divy"><a href="/dokumenty" class="patka_odkaz_web_divy_a">VÝVOJ</a></div></div></div>
	<div id="patka_2"><div id="patka_text" class="patka_div">
			<ul>
				<li class="bez_odrazky hlavni_sekce "><span class="podtrhnuto">AUTOŘI:</span> <ul><li class="bez_odrazky">Jakub Štěpánek: stepanek123@trebesin.cz</li>
				<li class="bez_odrazky">Tomáš Tarábek: tarabek123@trebesin.cz</li></ul></li>
				<li class="bez_odrazky hlavni_sekce"><span class="podtrhnuto">VEDOUCÍ PRÁCE:</span> <ul>
					<li class="bez_odrazky">Ing. Lukáš Jacečko: jacecko@trebesin.cz</li>
				</ul></li>
				
			</ul>
			
		</div>
		<div id="patka_logo" class="patka_div"><div class="patka_loga_R"><img src="svetlo.png" alt="intenzita" class="patka_loga_R_paranetry"><img src="teplota.png" alt="teplota" class="patka_loga_R_paranetry"><img src="tlak.png" alt="tlak" class="patka_loga_R_paranetry"><img src="vlhkost.png" alt="vlhkost" class="patka_loga_R_paranetry"></div><div class="patka_loga_L"><a href="/"><img src="logo_meteostanice.png" alt="Logo meteostanice" id="logo_meteostanice"></a><a href="https://www.trebesin.cz"target="_blank"><img src="trebesin_logo.png" alt="Logo Třebešín" id="logo_trebesin"></a></div></div>
</div>
	<div id="patka_3"><div class="patka_3" id="patka_3_loga">
	<div class="div_socky_basic"><a class="socky_img_a" href="https://www.instagram.com/prumyslovka_trebesin/" target="_blank"><img src="instagram.svg" alt="Školní instagram" class="socky_img">Školní instagram</a></div>
	<div class="div_socky_basic"><a href="https://www.facebook.com/trebesin/?locale=cs_CZ" class="socky_img_a"target="_blank"><img src="facebook.svg" alt="Školní facebook" class="socky_img">školní facebook</a></div>
	<div class="div_socky_basic"><a href="https://www.youtube.com/channel/UCeA7SCP5XHAwDmbk42RdJPg" class="socky_img_a"target="_blank"><img src="youtube.svg" alt="školní youtube" class="socky_img">školnou youtube</a></div>
	<div class="div_socky_basic"><a href="https://www.linkedin.com/search/results/all/?keywords=st%C5%99edn%C3%AD%20pr%C5%AFmyslov%C3%A1%20%C5%A1kola%20a%20gymn%C3%A1zium%20na%20t%C5%99ebe%C5%A1%C3%ADn%C4%9B&origin=RICH_QUERY_SUGGESTION&heroEntityKey=urn%3Ali%3Aorganization%3A18129325&position=0" class="socky_img_a"target="_blank"><img src="linkedin.svg" alt="Školní linkedin" class="socky_img">školní linkedin</a></div>
	<div class="div_socky_basic"><a href="https://www.instagram.com/jakub_stepanek_14/" class="socky_img_a"target="_blank"><img src="instagram.svg" alt="Kubův instagram" class="socky_img">Štěpánek instagram</a></div>
	<div class="div_socky_basic"><a href=" https://www.linkedin.com/in/jakub-%C5%A1t%C4%9Bp%C3%A1nek-74839b396/" class="socky_img_a"target="_blank"><img src="linkedin.svg" alt="Kubův linkedin" class="socky_img">Štěpánek linkedin</a></div>
<div class="div_socky_basic"><a href="https://www.instagram.com/tomas_tarabek/" class="socky_img_a"target="_blank"><img src="instagram.svg" alt="Tomův IG" class="socky_img">Tarábek instagram</a> </div>
<div class="div_socky_basic"><a href="https://www.linkedin.com/in/tom%C3%A1%C5%A1-tar%C3%A1bek-a05b54398/" class="socky_img_a"target="_blank"><img src="linkedin.svg" alt="Tomův linkedin" class="socky_img">Tarábek linkedin</a></div>
</div>

	
	<div class="patka_3" id="div_2026">2026</div></div>
		
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
		width: 100%;
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
	:global(html){
		scroll-behavior: smooth;
	}
	#patka{
		width: auto;
		min-height: 25rem;
		background-color:  #06d6a0;
		display: block;
		gap: 10px;
		padding: 1% 5% 1% 5%;
		max-width: 100vw;
		
		
	}
	#patka_text{
		
		/* border: 1px black solid; */
		padding-top: 2%;
		padding-left: 3%;
		color: black;
		font-family: var(--font-base);
		font-size: medium;
		height: 10%;
		
	}
	#patka_logo{
		/* border: 1px aqua solid; */
		display: flex;
		
		/* justify-content: ; */
		/* margin-left: 0.5%; */
		margin-bottom: 0;
		flex-wrap: wrap;
		flex-direction: row-reverse;
		gap: 12%;
		


	}
	#logo_trebesin{
		max-width: 20vw;
		transition: transform 2s ease;
	}
	#logo_trebesin:hover{
		transform: scale(1.2);
	}
	#logo_meteostanice{
		
		max-width: 20vw;
		transition: transform 2s ease;

	}
	#logo_meteostanice:hover{
		transform: scale(1.2);

	}
	.patka_loga_L{
		/* border: red dashed 2px; */
		display: flex;
		flex-direction: column;
		/* justify-content: space-around; */
		padding-left: 0%;
		margin-right: 0;
		width: auto;
		height: auto;
		gap: 5rem;
		
		align-content: center;
	}
	.patka_loga_R{
		/* border: blue dashed 2px; */
		max-width: 5%;
		width: auto;
		display: flex;
		flex-direction: column;
		justify-content: space-around;
		align-items: end;
		align-content: center;
		
		padding: 0.5%;
		


	}
	.patka_loga_R_paranetry{
		max-height: 2.5rem;
		object-fit: contain;
		transition: transform 1s ease;
		
	}
	.patka_loga_R_paranetry:hover{
		transform: translateX(-1.2rem);
	}
	.patka_div{
		width:100% ;
	}
	.bez_odrazky{
		list-style-type: none;
		font-size: 1rem;
		padding-left: 1rem;
		padding-bottom: 0.6rem;
		padding-top: 0.8rem;
	}
	.podtrhnuto{
		text-decoration: underline;
		font-size: 1.2rem;
		font-weight: 500;
		
		
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
		border-top: black 1px solid;
		min-height: 5rem;
		gap: 2rem;
		margin-top: 1rem;
		margin-right:5rem ;
		margin-left:5rem ;
	}
	#patka_3_loga{
		/* border: blue 1px solid; */
		display: flex;
		flex-direction: row;
		justify-content: space-evenly;
	}
	#div_2026{
		/* border: yellow 1px solid; */
		min-height: 2rem;
	}
	.div_socky_basic{
		min-height: 1rem;
		min-width: 2rem;
		max-height: 5rem;
		max-width: 5rem;
		
		/* border: red solid 1px; */
		/* IG, Facebook, youtube, linkein, IG osobni * 2 */
		/* div ve kterem jsou loga */
	}
	.socky_img{
		height: 3rem;
		aspect-ratio: 1;
/* pouze loga socek */
	}
	.socky_img_a{ 
/* pouze element a - tvorba odkazu a pak asi i animace */
		aspect-ratio: 1;
		color: inherit;
		text-decoration: none;
		font-size: 0.6rem;
		display: flex;
		flex-direction: column;
	}
	.socky_img_a:hover{
		cursor: pointer;
	}
	.socky_img_a img{
		transition: transform 0.5s ease;
		

	}
	.socky_img_a img:hover{
		transform: translateY(-0.5rem) rotate(5deg);
	
		
		filter: brightness(1.1);
	}
	#patka_2{
		display: flex;
	}
	
	#nadpis_patky{
		font-family: var(--font-mono);
		font-size: 2rem;
		font-weight: 500;
	}
	#patka_odkazy_web{
		padding-bottom: 1rem;
		margin-left: 5rem;
		margin-right: 5rem;
		margin-top: 1rem;
		border-bottom: black solid 1px;
		min-height: 3rem;
		display: flex;
		flex-direction: row;
		justify-content: space-evenly;
		align-items: end;
		
	}
	.patka_odkaz_web_divy{
		display: flex;
		width: 10rem;
		height: auto;
		/* border: aqua 2px dashed; */
		/* align-items: end; */
		justify-content: center;
		
		
	}
	.patka_odkaz_web_divy_a{
		text-decoration: none;
		color: inherit;
		font-weight: 500;
		transition: transform 1s ease;
		transform: scale(1.15);
	}
	.patka_odkaz_web_divy_a:hover{
		transform: scale(1.5) rotate(5deg) translateY(-0.1rem);

	}
	#patka_1{
		margin-bottom: 2rem;
	}
	@media( max-width:768px){
		#patka_logo{
		/* border: 1px aqua solid; */
		display: flex;
		
		/* justify-content: ; */
		/* margin-left: 0.5%; */
		margin-bottom: 0;
		flex-wrap: wrap;
		flex-direction: column;
		gap: 12%;
		


	}
	}

</style>