<script lang="ts">

const date = new Date();

</script>
<footer class="bg-orange-500 px-12 py-8 pb-12 w-full relative flex items-start gap-4 justify-around md:flex-col md:items-center">
    <div class="">
        <img class="w-[8rem] h-[8rem] mx-auto" src="./img/logo.png" alt="">
        <p class="text-black font-normal text-lg">Move the paper out and they read</p>
    </div>
    <div class="flex gap-12">
        <div class="">
            <h2 class="text-lg font-medium py-3">Useful Links</h2>
            <div class="flex flex-col text-gray-300 font-light">
                <a href="/">Home</a>
                <a href="#/about">About</a>
                <a href="#/contact">Contact</a>
                <a href="#/donate">Donate</a>
            </div>
        </div>
        <div class="">
            <h2 class="text-lg font-medium py-3">Get in touch</h2>
            <div class="flex flex-col text-gray-300 font-light">
                <a href="/">info@girlsofdestiny.rw</a>
                <a href="#/about">Twitter</a>
                <a href="#/contact">Facebook</a>
                <a href="#/donate">Youtube</a>
            </div>
        </div>
    </div>
    <div class="">
        <iframe class="" title="map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15955.635715203329!2d30.385134123262567!3d-1.2233332357232978!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x19dbeef6953faf55%3A0xe9411f5acae1ee2e!2sRwimiyaga!5e0!3m2!1sen!2srw!4v1665671924642!5m2!1sen!2srw" width="600"  allowfullscreen={true} loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>

    <p class="absolute text-sm text-gray-800 bottom-2">Copyright &copy; {date.getFullYear()} <strong>Girls Of Destiny</strong> all rights reserved.</p>
</footer>