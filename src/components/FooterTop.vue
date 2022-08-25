<template>
  <section class="container pt-5 pb-5 text-white">
    <div class="row">
      <ul class="col-3">
        <li class="list-title pb-4"><a href="#"><img id="footer-logo" src="../assets/img/logo-default.png" alt="iAcademy Logo"></a></li>
        <li class="base-text pb-4 text-capitalize">providing life changing experiences through education. class that fit your busy life. closer to home</li>
        <li class="pb-4"><FontAwesomeIcon class="footer-list-icon" icon="fa-solid fa-phone" /> <span class="footer-icon-indicator"> 1-677-124-44227</span></li>
        <li class="pb-4"><FontAwesomeIcon class="footer-list-icon" icon="fa-solid fa-clock" /> <span class="footer-icon-indicator"> Mon - Sat 08:00 - 18:00</span></li>
      </ul>

      <ul class="col-3">
        <li class="list-title pb-4">Popular Courses</li>
        <li class="pb-4">
          <h5 class="base-title">Business English</h5>
          <span class="base-text">Preston Marshall</span>
        </li>
        <li class="pb-4">
          <h5 class="base-title">Social Computing</h5>
          <span class="base-text">David Sanders</span>
        </li>
        <li class="pb-4">
          <h5 class="base-title">Learn Spanish</h5>
          <span class="base-text">Jennie King</span>
        </li>
      </ul>

      <ul class="col-3">
        <li class="list-title pb-4">Support</li>
        <li class="pb-4 base-text">User Dashboard</li>
        <li class="pb-4 base-text">Contact Us</li>
        <li class="pb-4 base-text">FAQ</li>
        <li class="pb-4 base-text">Course Offer</li>
        <li class="pb-4 base-text">Events</li>
      </ul>

      <ul class="col-3 text-end">
        <li class="list-title pb-4">Flexible Learning</li>
        <li><img id="world-map" src="../assets/img/world.png" alt="World Map"></li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
    name: 'FooterTop'
}
</script>

<style scoped lang="scss">
@import '../assets/sass/colours';
@import '../assets/sass/utils';

 section{  

  border-bottom: 1px solid $border_colour;

  #footer-logo{
    filter: invert(100%) sepia(54%) saturate(2%) hue-rotate(181deg) brightness(250%) contrast(101%);
    height: 2rem;
  }

  .base-text {
    font-weight: 100;
    font-family: sans-serif;
    color: $text_colour;
  }

  .footer-list-icon {
    padding-right: 0.2rem;
  }

  .footer-icon-indicator {
    font-size: 0.8rem;
    font-weight: 100;
  }

  .list-title{
    font-size: 1.5rem;
    font-weight: 600;
  }

  .base-title {
    font-size: 1.2rem;
    color: $text_colour;
    font-weight: 600;
  }

  #world-map{
    width: 14rem;
  }
 }
</style>