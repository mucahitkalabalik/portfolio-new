<template>
  <div id="profil">
    <div class="image-container">
      <img
        src="../../assets/images/profil2.png"
        height="150px"
        alt=""
        srcset=""
      />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#profil {
  padding-top: 200px;
  @media screen and (max-width: $medium) {
    padding-top: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .image-container {
    display: flex;
    align-items: center;
    justify-content: center;
    background: #c1ebfe;
    height: 250px;
    width: 250px;
    margin-left: 100px;
    border-radius: 50%;
    box-shadow: rgba(0, 195, 255, 0.56) 0px 22px 70px 4px;
    margin-left: 0px;
    animation: profil 2.5s infinite;
  }
}
@keyframes profil {
  0% {
    box-shadow: rgba(0, 195, 255, 0.7) 0px 22px 70px 4px;
  }
  50% {
    box-shadow: rgba(0, 195, 255, 0.01) 0px 22px 70px 4px;
  }
  100% {
    box-shadow: rgba(0, 195, 255, 0.7) 0px 22px 70px 4px;
  }
}
</style>