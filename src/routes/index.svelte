<script>
    import Goals from "../lib/Goals.svelte"
    import Tools from "../lib/Tools.svelte"
    import Process from "../lib/Process.svelte"
    import Portfolio from "../lib/Portfolio.svelte"

    var menuOption = "Goals"
</script>

<div class="w-screen h-screen bg-white">
    <div class="flex flex-col w-full h-1/2 bg-gray-800 rounded-b-2xl gap-6 items-center justify-center">
        <a class="flex justify-center text-[#175EB0] text-xl" target="_blank" href="https://goodfaithenergy.com/">
            <img class="w-2/3 md:w-1/4" src="/logo-name-blue-green.png" alt="GFE Logo"/>
        </a>
        <p class="text-white text-sm md:text-3xl text-center font-thin">INTERNSHIP 2022  -  MITCHELL HESS  -  IT/SOFTWARE DEVELOPMENT</p>
        <div class="w-5/6 h-0.5 rounded-full bg-gray-200"></div>
        <div class="w-3/4 h-1/4 md:h-1/3 bg-white rounded-xl shadow-[0px_0px_20px_0_rgba(0,0,0,0.3)]">
            <div class="flex flex-row w-full h-full rounded-xl relative">
                <button on:click={() => {menuOption="Goals"}} class="{menuOption === "Goals" ? "text-white" : "text-[#175EB0] hover:text-gray-800"} font-thin z-10 w-full h-full text-xs text-center md:text-[2.5rem] rounded-xl">
                    GOALS
                </button>
                <button on:click={() => {menuOption="Tools"}} class="{menuOption === "Tools" ? "text-white" : "text-[#175EB0] hover:text-gray-800"} font-thin z-10 w-full h-full text-xs text-center md:text-[2.5rem] rounded-xl">
                    TOOLS
                </button>
                <button on:click={() => {menuOption="Process"}} class="{menuOption === "Process" ? "text-white" : "text-[#175EB0] hover:text-gray-800"} font-thin z-10 w-full h-full text-xs text-center md:text-[2.5rem] rounded-xl">
                    PROCESS
                </button>
                <button on:click={() => {menuOption="Portfolio"}} class="{menuOption === "Portfolio" ? "text-white" : "text-[#175EB0] hover:text-gray-800"} font-thin z-10 w-full h-full text-xs text-center md:text-[2.5rem] rounded-xl">
                    PORTFOLIO
                </button>
                <div class="{menuOption==="Goals"?"left-0":""}{menuOption === "Tools"?"left-1/4":""}{menuOption === "Process"?"left-1/2":""}{menuOption === "Portfolio"?"left-3/4":""}
                    transition-all rounded-xl absolute top-0 w-1/4 h-full bg-gray-600 shadow-[0px_0px_20px_0_rgba(0,0,0,0.3)]"></div>
            </div>
        </div>
    </div>
    <div class="w-full md:h-[46.3rem] bg-white p-5 pb-10 md:pb-5">
        {#if menuOption === "Goals"}
            <Goals/>
        {:else if menuOption === "Tools"}
            <Tools/>
        {:else if menuOption === "Process"}
            <Process/>
        {:else}
            <Portfolio/>
        {/if}
    </div>
</div>
