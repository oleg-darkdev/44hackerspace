<script>
  import { CarouselTransition } from 'flowbite-svelte'
//   import { images } from './imageData/+server.js';
  import { bounceInOut } from 'svelte/easing';

export let bg = ''
</script>
    
<section style="" class="{bg}">

</section>

<style> 
.main-route {
  background-image: url(/banner.png);
}

.library-route {
  background-image: url(/banner_library.png);

}
section {
  /* Location of the image */  
  width: 100%;
  height: 500px;
  
  /* Image is centered vertically and horizontally at all times */
  background-position: center center;
  
  /* Image doesn't repeat */
  background-repeat: no-repeat;
  
  /* Makes the image fixed in the viewport so that it doesn't move when 
     the content height is greater than the image height */
  background-attachment: fixed;
  
  /* This is what makes the background image rescale based on its container's size */
  background-size: cover;
  
  /* Pick a solid background color that will be displayed while the background image is loading */
  background-color:#464646;
  
  /* SHORTHAND CSS NOTATION
   * background: url(background-photo.jpg) center center cover no-repeat fixed;
   */
}

/* For mobile devices */
@media only screen and (max-width: 767px) {
  .library-route  {
    background-image: url();
  }
  .main-route {
    background-image: url();
  }
  
}

</style>