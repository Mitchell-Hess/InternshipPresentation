<script>
    var step = 0
</script>

<div class="w-full h-[56rem] md:h-full grid grid-rows-5 md:grid-rows-3 grid-cols-2 md:grid-cols-3 gap-4 md:gap-8 md:p-16">
    <!--1st square-->
    <button on:click={() => {step === 1 ? step=0 : step=1}} class="{step===1?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] relative">
        <img class="hidden md:flex absolute w-1/3 -right-28 -top-10" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===1?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">1</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/gitea.png" alt="gitea"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===1?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Configuration</p>
        </div>
    </button>

    <!--2nd square-->
    <button on:click={() => {step === 2 ? step=0 : step=2}} class="{step===2?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] relative">
        <img class="hidden md:flex absolute w-1/3 -right-28 -top-10" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===2?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">2</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/nodeLogo.png" alt="node"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===2?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Project Setup</p>
        </div>
    </button>

    <!--3rd square-->
    <button on:click={() => {step === 3 ? step=0 : step=3}} class="{step===3?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] relative">
        <img class="hidden md:flex w-1/3 rotate-90 absolute -right-28 -bottom-6" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===3?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">3</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/figmaLogo.png" alt="figma"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===3?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Mockup and Design</p>
        </div>
    </button>

    <!--4th square-->
    <button on:click={() => {step === 8 ? step=0 : step=8}} class="{step===8?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 hidden md:flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)]">
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===8?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">8</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full bg-gray-300 overflow-hidden p-2">
                <img class="w-full h-full" src="process/deployment.png" alt="deployment"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===8?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Deployment</p>
        </div>
    </button>
    <button on:click={() => {step === 4 ? step=0 : step=4}} class="{step===4?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 flex md:hidden flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 rotate-90 absolute -right-28 -bottom-6" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===4?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">4</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/userInterface.png" alt="UI"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===4?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">User-interface Implementation</p>
        </div>
    </button>


    <!--Center Info-->
    <div class="flex w-full h-full row-span-1 md:row-span-1 col-span-2 md:col-span-1 text-xl md:text-3xl font-thin text-gray-800 items-center justify-center text-center">
        {#if step===1}
            <p>Initialized git repository, and added configuration files for tailwind, git, etc.</p>
        {:else if step===2}
            <p>Created frontend folder and installed svelte, created backend folder and installed npm and graphql, and created docker files for each.</p>
        {:else if step===3}
            <p>Used Dribbble for design ideas, and created a full mockup design on Figma.</p>
        {:else if step===4}
            <p>Programmed the user interface in the frontend folder based on the Figma design.</p>
        {:else if step===5}
            <p>Implemented datbases with prisma and graphql to store data for users, estimates, login sessions, etc.</p>
        {:else if step===6}
            <p>Added features such as estimate sharing, math implementation, and real-time updates.</p>
        {:else if step===7}
            <p>Fixed bugs (scrolling issues, formatting, math correction, etc) and made final changes</p>
        {:else if step===8}
            <p>Deployed website to phaseone.goodfaithenergy.com</p>
        {:else}
            <p>Click on a step to see more details</p>
        {/if}
    </div>

    <!--5th square-->
    <button on:click={() => {step === 4 ? step=0 : step=4}} class="{step===4?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 hidden md:flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 rotate-90 absolute -right-28 -bottom-6" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===4?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">4</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/userInterface.png" alt="UI"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===4?"text-white":""} md:text-[2.3rem] font-thin text-gray-800 text-center">User-interface Implementation</p>
        </div>
    </button>
    <button on:click={() => {step === 5 ? step=0 : step=5}} class="{step===5?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 md:hidden flex flex-col md:flex-row justify-items-center items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 rotate-180 absolute -left-28 -bottom-10" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===5?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">5</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/graphql.png" alt="graphql"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===5?"text-white":""}text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Backend and Database Connection</p>
        </div>
    </button>

    <!--6th square-->
    <button on:click={() => {step === 7 ? step=0 : step=7}} class="{step===7?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 hidden md:flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 -rotate-90 absolute -left-28 -top-6" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===7?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">7</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full bg-blue-300 overflow-hidden p-1.5">
                <img class="w-full h-full" src="process/bugFix.png" alt="bugFix"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===7?"text-white":""} md:text-[2.3rem] font-thin text-gray-800 text-center">Bug Fixes and UI Changes</p>
        </div>
    </button>
    <button on:click={() => {step === 6 ? step=0 : step=6}} class="{step===6?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 md:hidden flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 rotate-180 absolute -left-28 -bottom-10" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===6?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">6</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/checklist.png" alt="checklist"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===6?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Feature Implementation</p>
        </div>
    </button>

    <!--7th square-->
    <button on:click={() => {step === 6 ? step=0 : step=6}} class="{step===6?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 hidden md:flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 rotate-180 absolute -left-28 -bottom-10" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===6?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">6</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/checklist.png" alt="checklist"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===6?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Feature Implementation</p>
        </div>
    </button>
    <button on:click={() => {step === 7 ? step=0 : step=7}} class="{step===7?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 md:hidden flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 -rotate-90 absolute -left-28 -top-6" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===7?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">7</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full bg-blue-300 overflow-hidden p-1.5">
                <img class="w-full h-full" src="process/bugFix.png" alt="bugFix"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===7?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Bug Fixes and UI Changes</p>
        </div>
    </button>

    <!--8th square-->
    <button on:click={() => {step === 5 ? step=0 : step=5}} class="{step===5?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 hidden md:flex flex-col md:flex-row justify-items-center items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)] md:gap-4 relative">
        <img class="hidden md:flex w-1/3 rotate-180 absolute -left-28 -bottom-10" src="/process/arrow.png" alt="arrow"/>
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===5?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">5</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full overflow-hidden">
                <img class="w-full h-full" src="process/graphql.png" alt="graphql"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===5?"text-white":""} md:text-[2.3rem] font-thin text-gray-800 text-center">Backend and Database Connection</p>
        </div>
    </button>
    <button on:click={() => {step === 8 ? step=0 : step=8}} class="{step===8?"bg-gray-800":"hover:shadow-[0_0px_20px_0_rgba(0,0,0,0.5)]"} p-2 md:p-5 md:hidden flex flex-col md:flex-row items-center w-full h-full row-span-1 col-span-1 rounded-xl shadow-[0_0px_20px_0_rgba(0,0,0,0.3)]">
        <div class="w-full md:w-auto justify-around flex flex-row md:flex-col md:pb-5 items-center">
            <p class="{step===8?"text-white":""} text-[3rem] md:text-[4rem] font-thin text-gray-800 text-center">8</p>
            <div class="w-12 md:w-16 h-12 md:h-16 rounded-full bg-gray-300 overflow-hidden p-2">
                <img class="w-full h-full" src="process/deployment.png" alt="deployment"/>
            </div>
        </div>
        <div class="flex w-full h-full justify-center items-center">
            <p class="{step===8?"text-white":""} text-lg md:text-[2.3rem] font-thin text-gray-800 text-center">Deployment</p>
        </div>
    </button>
</div>