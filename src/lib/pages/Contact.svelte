<script lang="ts">
  import Anchor from "$lib/components/Anchor.svelte";
  import Text from "$lib/components/Text.svelte";
  import {primaryBackground} from "$lib/utils/constants";
  let phoneNumber1 = "972-881-7463"
  let phoneNumber2 = "469-661-9165"

  let email ="scplanotx@gmail.com";


 
  import { images } from '../utils/images2.js';
  let showThumbs=false
  let showCaptions=false
  import { Carousel } from 'flowbite-svelte'

</script>
<Anchor id="contact" />
<div
  class="flex flex-col items-center justify-center bg-center bg-no-repeat bg-cover page lg:bg-fixed bg-neutral-600 bg-blend-soft-light dark:bg-blend-soft-light dark:bg-neutral-700"
  id="bg">
<section class="relative py-20">
  <div class="bottom-auto top-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden -mt-20" style="height: 80px;">
    <svg class="absolute bottom-0 overflow-hidden" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none" version="1.1" viewBox="0 0 2560 100" x="0" y="0">
    </svg>
  </div>
    <div class="items-center flex flex-wrap">
      <div class="w-full  md:w-1/2 ml-auto mr-auto max-w-3xl">
       
       
<div class="container">
  <div
  class="relative flex flex-col min-w-0 break-words bg-white w-full mb-6 shadow-lg rounded-lg bg-slate-800"
  >
  <div class="max-w-4xl">
    <Carousel {images}  {showCaptions} {showThumbs} duration="3700"/>
  </div>
</div>  </div>





      </div>
  
      <div class="w-full md:w-5/12 ml-auto mr-auto px-4">
        <br>
        <div class="md:pr-12">
          <a href="mailto:{email}">
            <div class="text-white p-3 text-center inline-flex items-center justify-center w-16 h-16 mb-6 shadow-lg rounded-full bg-white">
              <svg width="24" height="24" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M24 21h-24v-18h24v18zm-23-16.477v15.477h22v-15.477l-10.999 10-11.001-10zm21.089-.523h-20.176l10.088 9.171 10.088-9.171z" />
              </svg>
              <i class="fas fa-rocket text-xl"></i>
            </div>
          </a>
          <a href="tel:{phoneNumber1}">
            <div class="text-white p-3 text-center inline-flex items-center justify-center w-16 h-16 mb-6 shadow-lg rounded-full bg-white">
              <svg width="24" height="24" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M18 24h-12c-1.104 0-2-.896-2-2v-20c0-1.104.896-2 2-2h12c1.104 0 2 .896 2 2v20c0 1.104-.896 2-2 2zm1-5.083h-14v3.083c0 .552.449 1 1 1h12c.552 0 1-.448 1-1v-3.083zm-7 3c-.553 0-1-.448-1-1s.447-1 1-1c.552 0 .999.448.999 1s-.447 1-.999 1zm7-17h-14v13h14v-13zm-1-3.917h-12c-.551 0-1 .449-1 1v1.917h14v-1.917c0-.551-.448-1-1-1zm-4.5 1.917h-3c-.276 0-.5-.224-.5-.5s.224-.5.5-.5h3c.276 0 .5.224.5.5s-.224.5-.5.5z" />
              </svg>
              <i class="fas fa-rocket text-xl"></i>
            </div>
          </a>
          <h3 class="text-3xl font-semibold">Contact us today</h3>
          <p class="text-lg font-semibold leading-relaxed mt-4 mb-4 text-white"> You can be confident that you’re dealing with a professionals that can handle your shoe repair needs from design to completion.  Please give us a call today for a free, no cost consultation. </p>
          <p class="text-lg font-semibold leading-relaxed mt-4 mb-4 text-white"> We pride ourselves on superior workmanship, excellent customer service, and an endless commitment to detail. Our mission is to provide industry-leading customer satisfaction, and we’re doing just that. </p>
          <p class="mt-4 text-lg leading-relaxed text-gray-600">
            <br>
          <p class="text-lg font-bold leading-relaxed mt-0 mb-4 text-white"> Anthony Shoe Care is here to serve you. We welcome all inquiries and look forward to hearing from you </p>
          <ul class="list-none mt-6">
            <li class="py-2">
              <div class="flex items-center">
                <div>
                  <span class="text-xs font-semibold inline-block py-1 px-2 uppercase rounded-full text-blue-600 bg-blue-300 mr-3">
                    <i class="fas fa-fingerprint"></i>
                  </span>
                </div>
                <div>
                  <a class="text-white font-medium	hover:text-lg hover:text-blue-300" href="tel:{phoneNumber1}">{phoneNumber1} Parker & Premier Location</a>
                </div>
              </div>
            </li>

            <li class="py-2">
              <div class="flex items-center">
                <div>
                  <span class="text-xs font-semibold inline-block py-1 px-2 uppercase rounded-full text-blue-600 bg-blue-300 mr-3">
                    <i class="fas fa-fingerprint"></i>
                  </span>
                </div>
                <div>
                  <a class="text-white font-medium	hover:text-lg hover:text-blue-300" href="tel:{phoneNumber2}">{phoneNumber2}  Plano Bazaar Location</a>
                </div>
              </div>
            </li>

            <li class="py-2">
              <div class="flex items-center">
                <div>
                  <span class="text-xs font-semibold inline-block py-1 px-2 uppercase rounded-full text-blue-600 bg-blue-300 mr-3">
                    <i class="fab fa-html5"></i>
                  </span>
                </div>
                <div>
                  <a class="text-white font-medium	hover:text-lg hover:text-blue-300" href="mailto:scplanotx@gmail.com">{email}</a>
                </div>
              </div>
            </li>
           


            <li class="py-2">
              <div class="flex items-center">
                <div>
                  <span class="text-xs font-semibold inline-block py-1 px-2 uppercase rounded-full text-blue-600 bg-blue-300 mr-3">
                    <i class="fab fa-html5"></i>
                  </span>
                </div>
                <div>
                  <a class="text-white font-medium	hover:text-lg hover:text-blue-300" href="/locations"> Our  & directions </a>
                </div>
              </div>
            </li>

          </ul>
        </div>
      </div>
    </div>
</section>

</div>

<style>
  #bg{
    background-image: radial-gradient(circle,#2f384b, #2f384b,#2f384b);  
   }

.container {
  position: relative;
  width: 100%;
  user-select: none;
  overflow: hidden;
  border-radius: 10px;
  color:white;
}
	.container :global(.swipeable) {
		position: absolute;
		top: 0;
	}

 



</style>