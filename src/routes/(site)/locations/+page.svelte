<script>
     let GOOGLE_MAPS_KEY="AIzaSyAOPo_kCh7y5pSAD1CzNVLMJsUbUYF_XTE"
     import Text from "$lib/components/Text.svelte";
     export let Parker_location= "601 W Parker Rd #113, Plano, TX";
     export let plano_bazaar_location="1409 Jupiter Rd Plano, Texas 75074"; 
 </script>
 
 <Text>
 <div class="container">
     <div class="location_container">
         <h1 class="text-4xl m-6 white font-bold">Parker & Premier</h1>
         <p class="text-2xl m-2 font-semibold">601 W Parker Rd #113, Plano, TX</p>
         <iframe class="responsive-iframe"
             loading="lazy"
             allowfullscreen
             referrerpolicy="no-referrer-when-downgrade"
             src={`https://www.google.com/maps/embed/v1/place?key=${GOOGLE_MAPS_KEY}&q=${encodeURIComponent(Parker_location)}`}>
         </iframe>
     </div>
 
     <div class="location_container">
         <h1 class="text-4xl m-6 white font-bold">Plano Bazaar</h1>
         <p class="text-2xl m-2 font-semibold">1409 Jupiter Rd #405 Plano, Texas 75074</p>
         <p class="text-2xl m-2 font-semibold text-red-500"> *Shop Closing 7/26/24* </p>

         <iframe class="responsive-iframe"
             loading="lazy"
             allowfullscreen
             referrerpolicy="no-referrer-when-downgrade"
             src={`https://www.google.com/maps/embed/v1/place?key=${GOOGLE_MAPS_KEY}&q=${encodeURIComponent(plano_bazaar_location)}`}>
         </iframe>
     </div>
 </div>
 </Text>
 
 <style>
 .container {
     padding-top: 1rem;
     padding-bottom: 1rem;
 }
 
 .location_container {
     padding-bottom: 2rem;
 }
 
 .responsive-iframe {
     width: 100%;
     height: 400px; /* or use 'height: 50vw' for height relative to the width */
     border: 0;
 }
 </style>
 