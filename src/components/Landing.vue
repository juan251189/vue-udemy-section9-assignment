<template>

    <div class="jumbotron hero" id="home" style="margin-bottom:0px;padding-bottom:20px;background-color:#d33e3e;background-image:url(&quot;none&quot;);">
      <div class="container">
        <div class="row" style="margin-right:0px;margin-left:0px;">
          <div class="col-md-12 col-sm-12">
            <img class="img-circle img-responsive" data-aos="zoom-out" data-aos-duration="1650" style="width:300px;height:60%;padding:0px;padding-top:0px;margin:0px auto;/*border:2px solid;*/"
              :src="`${publicPath}img/cartoon-profile3.png`"></div>
          <div class="col-md-12 col-sm-12">
            <h1 class="text-center" data-aos="zoom-in" data-aos-duration="500" style="color:rgb(222,222,222);font-size:34px;">Juan David Gomez R.</h1>
            <h2 class="text-center" data-aos="fade-up" data-aos-delay="500" data-aos-once="true" style="color:rgb(222,222,222);">Web Developer</h2>
          </div>
        </div>

      </div><i class="glyphicon glyphicon-chevron-down tada animated infinite" style="text-align:center;width:100%;color:rgb(255,252,252);font-size:26px;" href="portfolio"></i>
    </div>



</template>

<script>

export default {
  data () {
    return {
      publicPath: process.env.BASE_URL
    }
  }


}


</script>

<style>
</style>
