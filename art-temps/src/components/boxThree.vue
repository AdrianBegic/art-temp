<template>
  <div class="box">
    <div class="text-holder">
      <h1 class="title-services">Restoration</h1>
      <p>
        I take great pride in my ability to bring back the lost beauty and life
        to works of art and their accompanying frames.    
      </p>
      <p> Although it may not be
        noticible on a day to day basis paintings do accumulate
        dirt,grime,fireplace smoke and dust particles that diminish their
        vibrancy and brilliance. </p>
        <p> Rips, loss of tension, paint chipping and
        mould can occur over long periods of storage. Old varnish can turn dark
        and become brittle over time obscuring brilliance and detail of the
        work. </p><span id="media-width">
        <p>You'll be surprised to see what can be done, no matter how
        poor it looks. I save works of art to be enjoyed by those who follow,
        </p>
        <p> GARY OWEN</p>
        </span>
    </div>
    <div class="img-holder-services">
      <img id="resto" src="@/assets/images/art-resto.webp" />
    </div>
  </div>
</template>
<script>
export default {
  name: "boxThree",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
img {
  max-width: 100%;
  max-height: 100%;
  min-width: 100%;
  min-height: 100%;
}

#resto {
  border-radius: 0px 5px 5px 0px;
}

p {
  font-size: 1.2em;
}

.box {
  background-color: #F3D7C1;
  width: 80vw;
  height: 70vh;
  margin: 0 auto;
  padding:0;
  border-radius: 5px;
}

.img-holder-services {
  float: right;
  width: 50%;
  height: 100%;
  padding: 0;
}

.text-holder {
  float: left;
  width: 50%;
  height: 100%;
  color: #4d4d4d;
  font-weight: 100;
  padding: 30px;
}

.title-services {
  padding: 2% 0% 2%;
}




@media only screen and (min-width: 768px) {
    /* tablets and desktop */
    .box{
    height: 80vh;
    width: 90vw;
  }
}

@media only screen and (max-width: 767px) {
    /* phones */
    .box{
    height: 100vh;
    border-radius: 0px;
  }

   .text-holder { 
    float: none;
    margin-right:0;
    width:100%;
    height: auto;  
    padding: 5%; 
  }

  .title-services {
    margin: 0 auto;
  }

  .img-holder-services{
    height: 50%;
    width:100%;
  }

#resto {
  border-radius: 0px 0px 0px 0px;
}

  #media-width{
    display: none;
  }
}

@media only screen and (max-width: 767px) and (orientation: portrait) {
    /* portrait phones */
}

</style>
