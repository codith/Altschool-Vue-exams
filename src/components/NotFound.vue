<template>
  <div class="img-wrapper">
    <img src="@/assets/404svg.png" alt="404logo"/>
  </div>
  <div>
  <h1 class="heading">Sorry this page does not exist!!</h1>
  </div>
</template>

<script>
export default {
  name: "NotFound",
};
</script>

<style>

img{
  margin-left: 200px;
  align-items: center;
  justify-content: center;
  width: 200%;
  height:200%;
}
.img-wrapper {
  width: 100px;
  height: 100px;
}

.heading {
  font-size: 30px;
  margin-right: 200px;
  text-align: center;
  font-weight: lighter;
  font-family: primaryFont;
  object-fit: contain;
 
}

</style>
