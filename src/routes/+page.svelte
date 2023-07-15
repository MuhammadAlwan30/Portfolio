<script>
import "../app.css"
import Dark from "./components/dark.svelte";
</script>
    <body>
    <header class="flex justify-between lg:justify-around items-center h-1/4 min-w-[100vw] bg-gray-400">
        <div id="logo" class="p-4 mx-2 flex cursor-pointer"><img src="logo.svg" alt="logoimage" srcset="" class="mx-2">M. Alwan</div>
        <nav class="lg:w-60 hidden md:block lg:block">
            <ul class="flex flex-row w-full justify-between">
                <li class="inline-block hover:bg-gray-500 rounded-md p-1"><a href="#home">Home</a></li>
                <li class="inline-block hover:bg-gray-500 rounded-md p-1"><a href="#about">About</a></li>
                <li class="inline-block hover:bg-gray-500 rounded-md p-1"><a href="#Project">Project</a></li>
                <li class="inline-block hover:bg-gray-500 rounded-md p-1"><a href="blog">Blog</a></li>
            </ul>
        </nav>
        <div id="contact" class="hidden md:flex md:justify-center">
            <button class="bg-slate-500 p-2 rounded-full hover:bg-red-800 w-8 h-8"><img src="/moon.svg" alt="dark mode on"/></button>
            <a href="https://twitter.com/Cloudysdev" target="_blank" rel="noopener noreferrer">
                <button class="mx-4 bg-emerald-500 rounded-md p-1">contact</button>
        </a>
        </div>
        <div class="navbar block md:hidden lg:hidden m-3" id="navbar-button">
            <img src="bars-solid.svg" alt="click to navigate" width="16px">
        </div>
    </header>

    <!-- main area -->
    <section class="min-h-screen grid place-items-center bg-gray-300">
        <div class="m-2 p-2">
            <h1 class="text-left md:text-center">Hello I'm Alwan</h1>
            <h2>i'm front end developer from Indonesia where excited to learn about web technology</h2>
        </div>
    </section>
    <section class="min-h-screen block bg-gray-400">
        <h2 class="items-center">skills</h2>
        <div class="card-container w-full h-full">
            <div class="card bg-slate-300 max-w-lg mx-auto rounded-xl shadow-md overflow-hidden md:max-w-2xl">
                <div class="md:shrink-0"><img src="html-logo.png" alt="html logo" srcset=""></div>Html
            </div>
            <div class="card bg-gray-200 w-1/5 h-1/5">Css</div>
            <div class="card">Javasript</div>
            <div class="card">svelte</div>
            <div class="card"></div>
        </div>

        <p>currently learning about <span>Html</span> <span>Css</span> & javasript</p>
    </section>
    </body>
    <style lang="postcss">
    h1{
        font-size:4rem;
    }
    h2{
        font-size: 1.5em;
    }
    body{
        font-family:"fira mono", monospace;
    }
</style>
