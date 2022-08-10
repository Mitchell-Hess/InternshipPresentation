<script>
    var currentTool = "NONE"
</script>

<p class="text-3xl md:text-[3.5rem] text-gray-800 text-center font-thin">TOOLS USED</p>
<div class="w-full h-96 grid grid-rows-4 md:grid-rows-2 grid-cols-2 md:grid-cols-4 gap-4 py-4 rounded-xl">
    <button on:click={() => {currentTool === "DRIBBBLE" ? currentTool = "NONE" : currentTool = "DRIBBBLE"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]  overflow-hidden relative">
        <img class="w-full absolute bottom-0 md:-bottom-1/4"src="/tools/dribbble.png" alt="dribbble">
    </button>
    <button on:click={() => {currentTool === "FIGMA" ? currentTool = "NONE" : currentTool = "FIGMA"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)] overflow-hidden relative">
        <img class="absolute -bottom-3 md:-bottom-10"src="/tools/figma.png" alt="figma">
    </button>
    <button on:click={() => {currentTool === "DOCKER" ? currentTool = "NONE" : currentTool = "DOCKER"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)] overflow-hidden relative">
        <img class="w-full absolute -bottom-2 md:-bottom-10"src="/tools/docker.png" alt="docker">
    </button>
    <button on:click={() => {currentTool === "TAILWIND" ? currentTool = "NONE" : currentTool = "TAILWIND"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)] overflow-hidden relative">
        <img class="w-full absolute -bottom-4 md:-bottom-14"src="/tools/tailwind.png" alt="tailwind">
    </button>
    <button on:click={() => {currentTool === "SVELTE" ? currentTool = "NONE" : currentTool = "SVELTE"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)] overflow-hidden relative">
        <img class="w-full absolute -bottom-2 md:-bottom-10" src="/tools/sveltekit.png" alt="svelte">
    </button>
    <button on:click={() => {currentTool === "DRONE" ? currentTool = "NONE" : currentTool = "DRONE"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)] overflow-hidden relative">
        <img class="w-full h-full bottom-0 absolute md:bottom-0"src="/tools/drone.png" alt="drone">
    </button>
    <button on:click={() => {currentTool === "GIT" ? currentTool = "NONE" : currentTool = "GIT"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)] overflow-hidden relative">
        <img class="w-full absolute -bottom-3 md:-bottom-14"src="/tools/git.png" alt="git">
    </button>
    <button on:click={() => {currentTool === "NODE" ? currentTool = "NONE" : currentTool = "NODE"}} class="row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)] overflow-hidden relative">
        <img class="w-full absolute -bottom-1 md:-bottom-10"src="/tools/node.png" alt="node">
    </button>
</div>


<div class="{currentTool === "NONE" ? "max-w-0" : "max-w-[150rem]"} duration-300 z-10 flex flex-row w-full h-48 md:h-60 rounded-xl items-center shadow-[0_0px_20px_0px_rgba(0,0,0,0.3)] justify-around">
    <div class="flex md:w-1/3 h-full justify-center items-center">
        <p class="text-center text-lg md:text-[4rem] font-thin text-gray-800">{currentTool === "NONE" ? "" : currentTool }</p>
    </div>
    <div class="w-0.5 h-3/4 rounded-full bg-gray-800"></div>
    <div class="w-2/3 h-full flex flex-col p-2 md:p-10 justify-around items-center text-center">
        {#if currentTool === "DRIBBBLE"}
            <p class="text-xs md:text-3xl font-thin text-gray-800">With Dribbble, finding inspiration for website/app designs is simple. Serving as one of 
                the largest online platforms for designers to share their work, Dribbble provides countless options for almost any 
                website idea.</p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://dribbble.com/shots">Visit Dribble's website</a>
        {:else if currentTool === "FIGMA"}
            <p class="text-xs md:text-3xl font-thin text-gray-800">Before creating a functional website, it is important to design it. While Dribbble 
                is used for inspiration, Figma is used to create detailed mock-up designs to model what users will see.</p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://www.figma.com/?fuid=">Visit Figma's website</a>
        {:else if currentTool === "DOCKER"}
            <p class="text-xs md:text-2xl font-thin text-gray-800">Docker is a tool designed to make it easier to create, deploy, and run applications with 
                the help of containers. Containers allow a developer to compile up an application with all of the parts it needs, such 
                as libraries and other dependencies, and ship it all out as one single unit/package.</p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://www.docker.com/">Learn more about Docker</a>
        {:else if currentTool === "TAILWIND"}
            <p class="text-xs md:text-3xl font-thin text-gray-800">While HTML is used to create the actual content of a website, it is incomplete without
                CSS, which is used to style the HTML. TailwindCSS is a very beginner-friendly, yet efficient and practical CSS framework
                that helps with website styling.
            </p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://tailwindcss.com/">Learn more about TailwindCSS</a>
        {:else if currentTool === "SVELTE"}
            <p class="text-xs md:text-3xl font-thin text-gray-800">Svelte is a modern JavaScript framework used to build web apps that are fast, lean, and 
                fun for developers to use. You can use Svelte to build single, reusable components for projects of any kind.</p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://sveltekit.dev/">Learn more about Svelte</a>
        {:else if currentTool === "DRONE"}
            <p class="text-xs md:text-3xl font-thin text-gray-800">Drone is a continuous integration and delivery platform. Through integrations with many 
                popular version control services, you can use it to build, test, and deliver software automatically whenever your code 
                is updated.</p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://drone.goodfaithenergy.com/">Check out GFE's Drone platform</a>
        {:else if currentTool === "GIT"}
            <p class="text-xs md:text-3xl font-thin text-gray-800">Git is a DevOps tool used for source code management, and is for tracking changes in the 
                source code and enabling multiple developers to work together on non-linear development.</p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://git.goodfaithenergy.com/">Check out GFE's Git platform</a>
        {:else if currentTool === "NODE"}
            <p class="text-xs md:text-2xl font-thin text-gray-800">Node.js is an open source development platform for executing JavaScript code server-side. 
                Node is useful for developing applications that require a persistent connection from the browser to the server and is 
                often used for real-time applications such as chat, news feeds and web push notifications.</p>
            <a class="text-[#175EB0] text-sm md:text-xl" target="_blank" href="https://nodejs.org/en/about/">Learn more about Node.js</a>
        {/if}
    </div>
</div>