

<script>
//import { GOOGLE_MAPS_KEY } from  '$env/static/private'; //error when passed to a non +server.ts file    
// change key to open on https://console.cloud.google.com

   let GOOGLE_MAPS_KEY="AIzaSyAOPo_kCh7y5pSAD1CzNVLMJsUbUYF_XTE"


   /**
   * @type {any}
   */

   export let Parker_location= "601 W Parker Rd #113, Plano, TX";
     export let plano_bazaar_location="1409 Jupiter Rd Plano, Texas 75074"; 
    


    import Text from "$lib/components/Text.svelte";


</script>


  
<Text> 


<!-- svelte-ignore a11y-missing-attribute -->
<div class="container"> 



    <div class="location1_container"> 

    <h1 class="text-4xl m-6 white font-bold">Parker & premier</h1>
    <p class="text-2xl m-2 font-semibold">   601 W Parker Rd #113, Plano, TX </p> <br> 

    <iframe
  width="500"
  height="400"
  style="border:0"
  loading="lazy"
  allowfullscreen
  referrerpolicy="no-referrer-when-downgrade"
  src="https://www.google.com/maps/embed/v1/place?key={GOOGLE_MAPS_KEY}
    &q={Parker_location}">
</iframe>
</div>

<div class="location2_container"> 


    <h1 class="text-4xl m-6 white font-bold">Plano Bazaar </h1>
<p class="text-2xl m-2 font-semibold">  1409 Jupiter Rd #405 Plano, Texas 75074</p> <br> 

<iframe
  width="500"
  height="400"
  style="border:0"
  loading="lazy"
  allowfullscreen
  referrerpolicy="no-referrer-when-downgrade"
  src="https://www.google.com/maps/embed/v1/place?key={GOOGLE_MAPS_KEY}
    &q={plano_bazaar_location}">
</iframe>
</div>

<!-- svelte-ignore a11y-missing-attribute -->


</div>
</Text>


<style> 

.container{
    padding-top:1rem;
    padding-bottom:1rem;

}

.location1_container{
    padding-bottom:2rem;
}

.location2_container{
    padding-top:2.5rem;

}
</style>