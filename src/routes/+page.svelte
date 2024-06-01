<script>
	import { HtmlTag } from 'svelte/internal';
    import '../app.css';
    import Dark from './components/dark.svelte';
    // @ts-ignore
	let count = 0;
	function handleClick(){
		const menu = document.querySelector('.nav-links')
			menu?.classList.toggle("top-[9%]")
		console.log(menu?.classList[16])
	}
</script>

<body>
	<header class="bg-solid" id="head">
		<nav class="flex justify-between items-center w-[92%] mx-auto" id="navbar">
			<div id="logo" class="p-2 w-auto mx-2 flex cursor-pointer">
				<img src="logo.svg" alt="logoimage" srcset="" class="mx-2" />M.Alwan
			</div>
			<div class="nav-links absolute md:static bg-solid min-h-[60vh] md:min-h-fit left-0 top-[-100%] w-full md:w-auto flex items-center px-5 transition-all duration-500">
				<ul class="flex md:flex-row flex-col md:items-center md:gap-[4vw] gap-8">
					<li class="inline-block hover:border-black border-2 border-transparent rounded-md p-1">
						<a href="#home">Home</a>
					</li>
					<li class="inline-block hover:border-black border-2 border-transparent rounded-md p-1">
						<a href="#about">About</a>
					</li>
					<li class="inline-block hover:border-black border-2 border-transparent rounded-md p-1">
						<a href="#Project">Project</a>
					</li>
					<li class="inline-block hover:border-black border-2 border-transparent rounded-md p-1">
						<a href="blog">Blog</a>
					</li>
				</ul>
			</div>
			<div id="contact" class="hidden md:flex md:justify-center">
				<button class="bg-slate-500 p-2 rounded-full hover:bg-red-800 w-8 h-8">
                    <img src="/moon.svg" class="block ml-auto mr-auto w-1/2" alt="dark mode on" /></button>
				<a href="https://twitter.com/Cloudysdev" target="_blank" rel="noopener noreferrer">
					<button class="mx-4 bg-emerald-500 rounded-md p-1">contact</button>
				</a>
			</div>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<div class="navbar block md:hidden lg:hidden m-3 cursor-pointer" id="navbar-button" on:click={handleClick}>
				<img src="bars-solid.svg" alt="click to navigate" width="16px" />
			</div>
		</nav>
	</header>

	<!-- main area -->
	<section class="min-h-screen grid place-items-center bg-solid">
		<div class="m-2 p-2">
			<h1 class="text-left md:text-center">Hello I'm Alwan</h1>
			<h2>i'm front end developer from Indonesia where excited to learn about web technology</h2>
		</div>
	</section>

	<!-- about section -->
	<section id="about" class="min-h-screen bg-emerald-400 h-[95vh] w-full grid place-items-center">
		<div class="m-1 p-2">
			<h1 class="text-center">About</h1>
			<h2 class="indent-8">Experienced web developer with a passion for crafting elegant solutions in code. Two years of honing skills, building robust websites, and embracing the ever-evolving landscape of web development.
			</h2>
		</div>
		</section>

	<!-- skill section -->
	<section class="min-h-[100vh] block bg-gray-400">
		<h1 class="text-center">skills</h1>
		<div
			class="card-container m-auto mb-32 p-3 w-full max-w-2xl h-auto bg-solid flex justify-between flex-wrap rounded-xl">
			<div
				class="card-content w-40 h-40 bg-slate-300 flex flex-col p-3 m-2 justify-center border-2 border-black items-center rounded-xl hover:bg-blue-500 transition-colors duration-300"
			>
				<div class="w-16 h-16 md:w-24 md:h-24">
					<img src="html-logo.png" alt="html logo" srcset="" />
				</div>
				<div class="text-center">Html</div>
			</div>
			<div
				class="card-content w-40 h-40 bg-slate-300 flex flex-col p-3 m-2 border-2 border-black items-center hover:bg-blue-500 duration-300 rounded-xl"
			>
				Css
			</div>
			<div
				class="card-content w-40 h-40 bg-slate-300 flex flex-col p-3 m-2 border-2 border-black items-center hover:bg-blue-500 duration-300 rounded-xl"
			>
				Javasript
			</div>
			<div
				class="card-content w-40 h-40 bg-slate-300 flex flex-col p-3 m-2 border-2 border-black items-center hover:bg-blue-500 duration-300 rounded-xl"
			>
				svelte
			</div>
			<div
				class="card-content w-40 h-40 bg-slate-300 flex flex-col p-3 m-2 border-2 border-black items-center hover:bg-blue-500 duration-300 rounded-xl"
			>
				Tailwind
			</div>
			<div
				class="card-content w-40 h-40 bg-slate-300 flex flex-col p-3 m-2 border-2 border-black items-center hover:bg-blue-500 duration-300 rounded-xl"
			>
				React
			</div>
		</div>
	</section>

	
	<footer class="block bg-sky-500 text-center border-t-2 border-black rounded-t-2xl -mt-3 p-3 h-12">
		&copy; 2023 by Muhammad Alwan
	</footer>
</body>

<style lang="postcss">
	h1 {
		font-size: 4rem;
	}
	h2 {
		font-size: 1.5em;
	}
	body {
		font-family: 'fira mono', monospace;
	}
</style>

