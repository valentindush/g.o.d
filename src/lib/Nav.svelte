<script lang="ts">
    import FiFacebook from "svelte-icons-pack/fi/FiFacebook";
    import FiAtSign from "svelte-icons-pack/fi/FiAtSign";
    import FiInstagram from "svelte-icons-pack/fi/FiInstagram";
    import FiYoutube from "svelte-icons-pack/fi/FiYoutube";
    import FiTwitter from "svelte-icons-pack/fi/FiTwitter";
    import Icon from 'svelte-icons-pack'
</script>
<nav class="z-10 sm:absolute left-3">
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
    <div class="flex justify-between sm:flex-col">
        <div class="logo">
           <img src="./img/logo.png" class="w-12 h-12" alt="">     
        </div>
        <div class="nav-links">
            <ul class="flex gap-4 text-gray-200 sm:flex-col">
                <li><a href="/#/" class="p-2 hover:text-orange-500 duration-300 transition">Home</a></li>
                <li><a href="/#/about" class="p-2 hover:text-orange-500 duration-300 transition">About Us</a></li>
                <li><a href="/#/contact" class="p-2 hover:text-orange-500 duration-300 transition">Contact Us</a></li>
                <li><a href="/#/donate" class="p-2 hover:text-orange-500 duration-300 transition">Donate</a></li>
            </ul>
        </div>
        <div class="btn sm:mt-5">
            <a href="/#/donate" class="text-gray-200 text-d font-medium bg-orange-500 p-2 active:scale-[.98]">
               $ Donate
            </a>
        </div>
    </div>
</nav>