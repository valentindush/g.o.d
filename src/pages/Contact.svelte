<script lang="ts">
    import FiFacebook from "svelte-icons-pack/fi/FiFacebook";
    import FiAtSign from "svelte-icons-pack/fi/FiAtSign";
    import FiInstagram from "svelte-icons-pack/fi/FiInstagram";
    import FiYoutube from "svelte-icons-pack/fi/FiYoutube";
    import FiTwitter from "svelte-icons-pack/fi/FiTwitter";
    import HiOutlineMenuAlt2 from "svelte-icons-pack/hi/HiOutlineMenuAlt2";
    import AiOutlineClose from "svelte-icons-pack/ai/AiOutlineClose";
    import Icon from 'svelte-icons-pack'
  
  </script>
  <main class="">
      <header class="title mt-7 text-center md:texts">
          <h2 class="text-orange-500 text-2xl font-semibold">CONTACT US</h2>
          <p class="text-gray-300 text-sm mt-4">"Move the paper out and they read"</p>
      </header>
  
      <div class="text-center px-[8rem] md:px-1">
        <p class="text-gray-300 text-xl mt-12 opacity-70 ">
            We are always available to hear from your advices, We will respond to your feedback,
            also feel free to to talk to us for support of sponsorship.
            once we see it. DROP US A LINE.  
            <p>
      </div>

      <div class="form w-full h-fit p-4 bg-gray-100 rounded-lg mt-12 pb-5">
        <div class="flex gap-12 flex-wrap">
            <form action="#" class="w-[50%] min-w-[500px] md:min-w-full bg-white bg-opacity-50">
                <h2 class="text-xl font-medium text-gray-800 py-2 text-center">Contact us via email</h2>
                <input type="text" placeholder="Names" class="block border-2 border-orange-200 outline-none p-2 rounded-md w-full focus:border-orange-400 mt-3 px-4 font-normal text-sm text-gray-800 bg-white bg-opacity-50">
                <input type="email" placeholder="Your email address" class="block border-2 border-orange-200 outline-none p-2 rounded-md w-full focus:border-orange-400 mt-3 px-4 font-normal text-sm text-gray-800 bg-white bg-opacity-50">
                <textarea rows="8" placeholder="Message" class="block border-2 border-orange-200 outline-none p-2 rounded-md w-full focus:border-orange-400 mt-3 px-4 font-normal text-sm text-gray-800 resize-y bg-white bg-opacity-50"></textarea>
                <button class="bg-orange-500 text-white mt-3 p-2 w-full rounded-md">Send message</button>
            </form>
            <div class="w-[40%] mt-4 md:w-full md:text-center">
                <p class="py-2 text-md text-gray-800">girlsofdestiny2015@gmail.com</p>
                <div class="social flex gap-2">
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
                <p class="py-2 text-md text-gray-800">+250 788 415 849</p>
                <p class="py-2 text-md text-gray-800">Rwanda, eastern province, Nyagatare district, Rwimiyaga sector</p>
                <p class="py-2 text-2xl text-gray-800">“Move the paper out and they read”</p>
            </div>
            <div class="mt-4 md:mt-1 w-full md:w-full">
                <iframe class="w-full h-full" title="map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15955.635715203329!2d30.385134123262567!3d-1.2233332357232978!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x19dbeef6953faf55%3A0xe9411f5acae1ee2e!2sRwimiyaga!5e0!3m2!1sen!2srw!4v1665671924642!5m2!1sen!2srw" allowfullscreen={true} loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
        </div>
      </div>
         
  </main>