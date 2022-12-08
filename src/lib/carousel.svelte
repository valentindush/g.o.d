<script lang="ts">
    import FaSolidAngleLeft from "svelte-icons-pack/fa/FaSolidAngleLeft";
    import Icon from "svelte-icons-pack";
    import 'swiper/css/navigation';
    import 'swiper/css/pagination';
    import 'swiper/css/scrollbar';
    import { Navigation, Pagination, Scrollbar, A11y } from 'swiper';
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

    import {Swiper, SwiperSlide} from 'swiper/svelte';
    import 'swiper/css'

</script>
<div class="px-24 mt-4 py-6 relative md:px-1">
    <h2 class="text-2xl text-gray-700 font-semibold py-4 md:text-center">Take a look at some of our beautiful images</h2>   
 
    <Swiper
    modules={[Navigation, Pagination, Scrollbar, A11y]}
    spaceBetween={20}
    slidesPerView={3}
    navigation
    pagination={{ clickable: true }}
    on:slideChange={() => console.log('slide change')}
    on:swiper={(e) => console.log(e.detail[0])}
  >

  {#each images as image}
    <SwiperSlide>
      <img src={`./img/${image}`} alt="move the paper out and they read" class="w-full h-64 object-cover rounded-lg" />
    </SwiperSlide>
    {/each}
  </Swiper>
</div>