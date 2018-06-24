<template>
    <div class="main">
      <div class="container">
        <div class="image">
          <img src="../assets/images/img.jpg" alt="" srcset="">
        </div>
        <div class="name">Griffith Asare Awuah</div>
        <div class="about">FullStack Developer</div>
        <div class="ico-container">
          <a href="https://www.twitter.com/gwuah_"><i data-feather="twitter"></i></a> · 
          <a href="https://www.github.com/gwuah_"><i data-feather="github"></i></a> · 
          <a href='https://www.facebook.com/griffith.awuah.14'><i data-feather="facebook"></i></a>
        </div>
      </div>
    </div>
</template>

<style type="text/css" scoped>
  .name {
    font-weight: bold;
  }
  .name, .about {
    margin-bottom: 0px !important;
  }
  .ico-container {
    margin-top: 12px;
  }

  .ico-container svg {
    height: 20px !important;
    width: 20px !important;
    margin-right: 10px;
    margin-left: 10px;
  }
</style>

<script>
  export default {
    name: "Header",
    methods: {
      goto(url) {
        // console.log("goto", url);
        window.location.href = url;
      }
    },
    mounted: function() {
      // console.log(feather);
      feather.replace()
    }
  };
</script>
