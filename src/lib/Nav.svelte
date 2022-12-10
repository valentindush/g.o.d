<script lang="ts">
    import FiFacebook from "svelte-icons-pack/fi/FiFacebook";
    import FiAtSign from "svelte-icons-pack/fi/FiAtSign";
    import FiInstagram from "svelte-icons-pack/fi/FiInstagram";
    import FiYoutube from "svelte-icons-pack/fi/FiYoutube";
    import FiTwitter from "svelte-icons-pack/fi/FiTwitter";
    import HiOutlineMenuAlt2 from "svelte-icons-pack/hi/HiOutlineMenuAlt2";
    import AiOutlineClose from "svelte-icons-pack/ai/AiOutlineClose";
    import Icon from 'svelte-icons-pack'

    $:width = window.innerWidth;
   window.addEventListener('resize',()=>{
    width = window.innerWidth;
   })
   $:navActive = false;
   $:navClass =(width < 750) ? "block" : "hidden";
   const handleNav = ()=>{
        navActive = !navActive;
        navClass = navActive ? "block" : "hidden";
    }
</script>
<nav class="z-10 md:fixed mt-0 md:w-[40%] sm:w-[70%] fixed w-full px-2 pr-8 top-0 left-3 backdrop-blur-sm bg-white bg-opacity-10 shadow-md">

    {#if !navActive}
        <div on:click={handleNav} class="absolute hidden md:block mt-1 ml-1 cursor-pointer active:scale-105">
            <Icon src={HiOutlineMenuAlt2} color="gray" size="30" />
        </div>
        {:else}
            <div on:click={handleNav} class="absolute hidden md:block mt-1 ml-4 cursor-pointer active:scale-105">
                <Icon src={AiOutlineClose} color="gray" size="24"/>
            </div>
    {/if}
    
    <div class={`md:bg-gray-900 bg-opacity-40 md:p-5 rounded ${width < 750?navClass:""}`}>
        <div class="">
            <div class="social flex gap-2 items-center justify-center py-5">
                <a href="/#">
                    <Icon src={FiAtSign} color="gray" size="24" />
                </a>
                <a href="/#">
                    <Icon src={FiFacebook} color="gray" size="24" />
                </a> 
                <a href="/#">
                    <Icon src={FiInstagram} color="gray" size="24" />
                </a>
                <a href="/#">
                    <Icon src={FiTwitter} color="gray" size="24" />
                </a>
                <a href="/#">
                    <Icon src={FiYoutube} color="gray" size="24" />
                </a>
    
            </div>
        </div>
        <div class="flex justify-between md:flex-col">
            <div class="logo">
               <a href="/">
                <img src="./img/logo.png" class="w-12 h-12" alt="">   
               </a>  
            </div>
            <div class="nav-links">
                <ul class="flex gap-4 text-gray-400 md:flex-col">
                    <li><a href="/#/" class="p-2 hover:text-orange-500 duration-300 transition">Home</a></li>
                    <li><a href="/#/contact" class="p-2 hover:text-orange-500 duration-300 transition">Contact Us</a></li>
                    <li><a href="/#/donate" class="p-2 hover:text-orange-500 duration-300 transition">Donate</a></li>
                </ul>
            </div>
            <div class="btn md:mt-5">
                <a href="/#/donate" class="text-gray-800 hover:shadow-lg text-d font-medium bg-orange-500 p-2 px-5 active:scale-[.98]">
                   $ Donate
                </a>
            </div>
        </div>
    </div>
</nav>