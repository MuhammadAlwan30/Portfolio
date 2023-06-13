<script>
import "../app.css"
</script>
    <body>
    <header class="flex justify-between items-center h-1/4 min-w-[100vw]">
        <div id="logo" class="p-4 mx-2 flex cursor-pointer"><img src="logo.svg" alt="logoimage" srcset=""> Alwan</div>
        <nav class="w-60">
            <ul class="flex flex-row w-full justify-between">
                <li class="inline-block"><a href="#home">Home</a></li>
                <li class="inline-block"><a href="#about">About</a></li>
                <li class="inline-block"><a href="#Project">Project</a></li>
                <li class="inline-block"><a href="blog">Blog</a></li>
            </ul>
        </nav>
        <div id="contact">
            <a href="https://twitter.com/Cloudysdev" target="_blank" rel="noopener noreferrer">
                <button class="mx-4 bg-emerald-500 rounded-md p-1">contact</button>
        </a>
        </div>
    </header>
    <div id="wrapper">
        <h1>Hello I'm Alwan</h1>
        <h2>front end developer who enthusisast in web development and recent tech trends</h2>
    </div>
    </body>
    <style lang="postcss">
    h1{
        font-size:4rem;
    }
    body{
        background-color: #4c4cc1;
        font-family:"fira mono", monospace;
    }
    #wrapper{
        display: grid;
        place-items:center;
        min-height: 90vh;
        min-width: 100vw;
    }
</style>
