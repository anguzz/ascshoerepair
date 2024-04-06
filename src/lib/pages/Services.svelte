<script lang="ts">
  import Page from "$lib/components/Page.svelte";
  import Text from "$lib/components/Text.svelte";
  import { primaryBackground } from "$lib/utils/constants";
  import Anchor from "$lib/components/Anchor.svelte";
  export let backgroundClass = primaryBackground;
  
  
  let box1title="Repairs"
  let box1info="We offer complete boot and shoe repair, as well as belts, backpacks and purse repairs."
  
  let box2title="Alterations"
  let box2info="We can install orthropedic lifts, professinally stretch shoes and perform any other alterations."
  
  let box3title="Recrafts"
  let box3info="Shoes are stretched over their original lasts to retain shape and appearance, soles are replaced, welting, laces, and heels are replaced, and the uppers are refinished"

  import { images } from '../utils/images.js';
  import { Carousel  } from 'flowbite-svelte'
  let showThumbs=false
  let showCaptions=false

  
</script>
<Anchor id="services" />
<section class="pb-20 relative block bg-grey-900">
  <div
    class="bottom-auto top-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden -mt-20"
    style="height: 80px;"
    >
    <svg
      class="absolute bottom-0 overflow-hidden"
      xmlns="http://www.w3.org/2000/svg"
      preserveAspectRatio="none"
      version="1.1"
      viewBox="0 0 2560 100"
      x="0"
      y="0"
      >
      <polygon
        class="text-gray-900 fill-gray-300"
        points="2560 0 2560 100 0 100"
        ></polygon>
    </svg>
  </div>
</section>
<section class="pb-20 bg-gray-300 -mt-24">
  <div class="container mx-auto px-4">
    <div class="flex flex-wrap">
      <div class="lg:pt-12 pt-6 w-full md:w-4/12 px-4 text-center">
        <div
          class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
          >
          <div class="px-4 py-5 flex-auto">
            <div
              class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-red-400"
              >
              <svg fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
              width="24" height="24" viewBox="0 0 60.705 60.705"
              xml:space="preserve">
              <path d="M41.621,5.882c-2.965-1.306-6.748-1.941-11.565-1.941h-6.87v-1.58C23.185,1.056,22.127,0,20.824,0h-9.571
                C9.949,0,8.892,1.058,8.892,2.361v20.622c0,1.304,1.058,2.36,2.361,2.36h9.571c1.304,0,2.361-1.057,2.361-2.36v-1.279h0.914V29.7
                h-1.935c-1.304,0-2.361,1.057-2.361,2.36v26.283c0,1.305,1.058,2.361,2.361,2.361h16.376c1.306,0,2.361-1.059,2.361-2.361V32.061
                c0-1.304-1.059-2.357-2.361-2.357h-1.936v-7.931c3.195,0.188,6.365,0.998,11.229,5.563c0.447,0.419,1.027,0.64,1.617,0.64
                c0.315,0,0.637-0.064,0.938-0.194c0.862-0.374,1.424-1.228,1.424-2.168v-4.311C51.814,14.858,46.441,8.005,41.621,5.882z
                M36.18,55.984H24.527V34.423h1.934h7.785h1.935V55.984z M28.822,29.7v-7.208h3.061V29.7H28.822z M34.705,16.98h-13.88
                c-1.305,0-2.362,1.058-2.362,2.362v1.277h-4.847V4.721h4.847v1.581c0,1.306,1.058,2.362,2.362,2.362h9.23
                c4.146,0,7.311,0.504,9.662,1.54c3.162,1.394,6.949,6.201,7.342,10.399C42.462,17.432,38.81,17.061,34.705,16.98z"/>
            </svg>
              
              <i class="fas fa-award"></i>
            </div>
            <h6 class="text-xl font-semibold text-black">{box1title}</h6>
            <p class="mt-2 mb-4 text-gray-600">
              {box1info}
            </p>
          </div>
        </div>
      </div>
      <div class="w-full md:w-4/12 px-4 text-center text-black">
        <div
          class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
          >
          <div class="px-4 py-5 flex-auto">
            <div
              class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-blue-400"
              >
             
              <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <path d="M0 0v24h6v-24h-6zm4 22h-2v-2h1v-1h-1v-2h1v-1h-1v-2h1v-1h-1v-2h1v-1h-1v-2h1v-1h-1v-2h1v-1h-1v-2h2v20zm9-4.697l1.131 1.697h-1.131v-1.697zm-1-3.303v6h4l-4-6zm-4-14v24h16l-16-24zm2 20h1v-1h-1v-2h1v-1h-1v-2h1v-1h-1v-2h1v-1h-1v-3.026l10.392 15.026h-10.392v-2z"/>
              </svg>
              <i class="fas fa-retweet"></i>
            </div>
            <h6 class="text-xl font-semibold">{box2title}</h6>
            <p class="mt-2 mb-4 text-gray-600">
              {box2info}
            </p>
          </div>
        </div>
      </div>
      <div class="pt-6 w-full md:w-4/12 px-4 text-center">
        <div
          class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
          >
          <div class="px-4 py-5 flex-auto">
            <div
              class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-green-400"
              >
              <svg fill="#000000" height="30" width="30" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 500 500" xml:space="preserve">
               

                      <path d="M488,298.168v-20.432c0-34.104-6.816-67.272-20.24-98.592c-3.936-9.2-12.944-15.144-22.952-15.144     c-11.096,0-20.968,7.456-24.016,18.12l-4.248,14.864C412.672,210.528,400.128,220,386.032,220c-9.16,0-17.856-3.952-23.88-10.832     l-17.936-20.496l6.464-19.368c0.872-2.672,1.32-5.432,1.32-8.224V158c0-14.336-11.664-26-26-26c-5.592,0-11.136,1.848-15.592,5.2     l-25.56,19.168c-2.272-0.192-4.544-0.368-6.84-0.368c-15.928,0-31.432,4.552-44.84,13.168l-42.776,27.504     c-32.76,21.056-68.816,35.168-107.16,41.928l-42.272,7.464C17.224,250.248,0,270.784,0,294.88     c0,20.768,13.12,39.488,32.632,46.584C73.744,356.424,116.768,364,160.512,364H472c13.232,0,24-10.768,24-24v-6.112     C496,321.6,493.24,309.296,488,298.168z M350.112,219.696c9.056,10.36,22.152,16.304,35.92,16.304     c21.192,0,40.072-14.232,45.896-34.624l4.248-14.864c1.096-3.84,4.648-6.512,8.632-6.512c3.592,0,6.832,2.136,8.248,5.448     C465.624,214.768,472,245.816,472,277.736v15.12C453.368,294.864,399.544,300,336,300c-1.256,0-2.352,0.04-3.576,0.048     l-48.032-75.48c14.936-9.32,26.432-23.424,32.392-40.12c4.208,2.992,8.12,6.448,11.584,10.408L350.112,219.696z M244.464,240.28     l23.368-7.792c0.72-0.24,1.376-0.592,2.08-0.856l43.816,68.856c-10.24,0.432-19.448,1.112-27.784,2.008L244.464,240.28z      M268.224,304.76c-7.824,1.16-15.192,2.416-22.416,3.672c-2.744,0.488-5.472,0.96-8.216,1.424l-34.808-55.688l25.944-8.648     L268.224,304.76z M320.008,150c1.72-1.288,3.84-2,5.992-2c5.512,0,10,4.488,10,10v3.08c0,1.08-0.168,2.152-0.504,3.168     l-3.864,11.576c-7.736-6.576-16.536-11.672-26.032-15.024L320.008,150z M199.048,210.128l42.776-27.504     C252.64,175.672,265.16,172,278.008,172c8.472,0,16.736,1.696,24.448,4.728c-5.928,18.96-20.6,34.224-39.68,40.584l-94.88,31.624     c-13.336,4.448-27.968,4.016-41.016-1.2l-5.032-2.016C149.016,237.504,174.896,225.648,199.048,210.128z M43.744,261.816     l42.272-7.464c3.2-0.56,6.352-1.264,9.52-1.92l25.4,10.16c8.976,3.584,18.424,5.408,28.088,5.408     c8.144,0,16.184-1.304,23.92-3.88l14.232-4.744l33.232,53.168C205.752,314.568,189.464,316,168,316     c-58.744,0-129.52-22.152-150.864-29.312C20.296,274.112,30.456,264.16,43.744,261.816z M480,340c0,4.416-3.584,8-8,8H160.512     c-41.872,0-83.064-7.256-122.416-21.56c-10.4-3.784-18.04-12.464-20.856-22.832C43.976,312.36,110.36,332,168,332     c35.744,0,58.52-3.968,80.552-7.808C271.704,320.168,295.64,316,336,316c65.768,0,121.304-5.44,139.008-7.376     c3.216,8.024,4.992,16.632,4.992,25.264V340z"/>
                     
                   
                </svg>
            
              <i class="fas fa-fingerprint"></i>
            </div>
            <h6 class="text-xl font-semibold text-black">{box3title}</h6>
            <p class="mt-2 mb-4 text-gray-600">
              {box3info}
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="flex flex-wrap items-center mt-12">
      <div class="w-full md:w-5/12 px-4 mr-auto ml-auto">
        <h3 class="text-3xl mb-2 font-semibold leading-normal text-gray-700">
          Working with us is a pleasure
        </h3>
        <p
          class="text-xl font-bold leading-relaxed mt-4 mb-4 text-gray-700"
          >
          Anthony Shoe Repair is not just a shop; it's a legacy of craftsmanship and dedication. <br><br> As Texas' premier shoe care and leather specialty shop, we bring over 30 years of expertise to the table. <br><br> Our commitment to excellence and attention to detail have made us one of the most trusted professionals in the industry.  <br><br>Whether it's a cherished pair of boots or a beloved leather purse, we ensure that your items receive the utmost care and are restored to their pristine condition. </div>
      <div class="w-full md:w-4/12 px-4 mr-auto ml-auto">
        <div
          class="relative flex flex-col min-w-0 break-words bg-white w-full mb-6 shadow-lg rounded-lg bg-slate-800"
          >
          <div class="object-contain h-full w-full">
            <Carousel {images}  {showCaptions} {showThumbs} duration="3700"/>
          </div>
          <blockquote class="relative p-8 mb-4">
            <svg
              preserveAspectRatio="none"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 583 95"
              class="absolute left-0 w-full block"
              style="height: 95px; top: -94px;"
              >
              <polygon
                points="-30,95 583,95 583,65"
                class="text-slate-800 fill-current"
                ></polygon>
            </svg>
            <h4 class="text-xl font-bold text-white">
              Our Mission
            </h4>
            <p class="text-md font-semibold mt-2 text-white">
              We pride ourselves on exceptional craftsmanship, exceptional customer service, and superior attention to detail. Our mission is to provide our clients with utmost satisfaction.            </p>
          </blockquote>
        </div>
      </div>
    </div>
  </div>
</section>
<style></style>