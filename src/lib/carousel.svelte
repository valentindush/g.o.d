<script lang="ts">
    import FaSolidAngleLeft from "svelte-icons-pack/fa/FaSolidAngleLeft";
    import Icon from "svelte-icons-pack";
    const images:string[] = [
        'image1.png',
        'image2.png',
        'image3.png',
        'image4.png',
        'image1.png',
        'image2.png',
        'image3.png',
        'image4.png'
    ]

    let div:HTMLDivElement;
    
    const scrollLeft = ()=>{
        div.scroll({
            left: div.scrollLeft - 300,
            behavior: 'smooth'
        })
    }
    const scrollRight = ()=>{
        div.scroll({
            left: div.scrollLeft + 300,
            behavior: 'smooth'
        })
    }
</script>
<div class="px-24 mt-4 py-6 relative md:px-1">
    <h2 class="text-2xl text-gray-700 font-semibold py-4 md:text-center">Take a look at some of our beautiful images</h2>   
    <div class="px-0 md:px-7">
        <button on:click={scrollLeft} class="bg-gray-200 absolute w-12 h-12 flex items-center justify-center top-[40%] left-5 cursor-pointer active:scale-[.98] md:left-0 md:top-1/2 md:scale-75">
            <Icon src={FaSolidAngleLeft} color="gray" size="24" />
        </button>
        <button on:click={scrollRight} class="bg-gray-200 absolute w-12 h-12 flex items-center justify-center top-[40%] right-5 cursor-pointer active:scale-[.98] md:right-0 md:top-1/2 md:scale-75">
            <Icon src={FaSolidAngleLeft} color="gray" size="24" className='rotate-180' />
        </button>
        <div bind:this={div} class="flex gap-2 w-full overflow-hidden relative px-1">
            
            {#each images as img}
                <img class="w-[20rem] h-[14rem] object-cover" src={`./img/${img}`} alt="mover the paper out and they read">
            {/each}
        </div>
    </div>
</div>