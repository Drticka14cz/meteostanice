# Projekt MeteostanicA - doprovodný web
--------------------------------------
## Web k meteostanici bude obsahovat několik funkcí:
  - návod k použití meteostanice, vysvětlení schématu
  - popis projektu
  - bonus: 
    - výpis hodnot z meteostanice na web
    - interaktivní virtuální meteostanice (využití funkcí svelte)


## Návod k stažení  a spuštění:
  - stáhněte si tento repoitář do svého pc, buď ručně a nebo za využití gitu ve vašem vs codu (git init, git branch -m master main, git remote add origin <odkaz-na-tento-github>, git pull origin main)
  - po stáhnutí repozitáře napiště do terminálu následující příkazy(příkazy piště do místění repozitáře př.: c/user/meteostanice):
  
    - npm install (instalace npm - soubory důležité ke spuštění svelte projektu)
    - npm run dev -- --open  (zapnutí projektu - rovnou by mělo otevřít prohlížeč na portu kde je spuštěn svelte soubor. Pokud se to nespustí, v terminálu bude napsáno na jakém portu se to spustilo - pak jen do     prohlížeče napiště lockalhost:<číslo_portu>)
      
  - užívejete web :D




### Originální readme z dokumentace svelte:


# sv

Everything you need to build a Svelte project, powered by [`sv`](https://github.com/sveltejs/cli).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```sh
# create a new project
npx sv create my-app
```

To recreate this project with the same configuration:

```sh
# recreate this project
npx sv create --template minimal --no-types --install npm .
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```sh
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.
>
> fico
