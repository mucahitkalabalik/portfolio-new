<template>
  <section>
    <div class="infinity">
      <div class="circle">
        <span style="--i: 0"></span>
        <span style="--i: 2"></span>
        <span style="--i: 3"></span>
        <span style="--i: 4"></span>
        <span style="--i: 5"></span>
        <span style="--i: 6"></span>
        <span style="--i: 7"></span>
        <span style="--i: 8"></span>
        <span style="--i: 9"></span>
        <span style="--i: 10"></span>
        <span style="--i: 11"></span>
        <span style="--i: 12"></span>
        <span style="--i: 13"></span>
        <span style="--i: 14"></span>
        <span style="--i: 15"></span>
        <span style="--i: 16"></span>
        <span style="--i: 17"></span>
        <span style="--i: 18"></span>
        <span style="--i: 19"></span>
        <span style="--i: 20"></span>
      </div>
       <div class="circle">
        <span style="--i: 0"></span>
        <span style="--i: 2"></span>
        <span style="--i: 3"></span>
        <span style="--i: 4"></span>
        <span style="--i: 5"></span>
        <span style="--i: 6"></span>
        <span style="--i: 7"></span>
        <span style="--i: 8"></span>
        <span style="--i: 9"></span>
        <span style="--i: 10"></span>
        <span style="--i: 11"></span>
        <span style="--i: 12"></span>
        <span style="--i: 13"></span>
        <span style="--i: 14"></span>
        <span style="--i: 15"></span>
        <span style="--i: 16"></span>
        <span style="--i: 17"></span>
        <span style="--i: 18"></span>
        <span style="--i: 19"></span>
        <span style="--i: 20"></span>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
section {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 30vh;
  margin-top: 200px;
}
.infinity {
  display: flex;
}
.circle {
  position: relative;
  width: 200px;
  height: 200px;
  margin: 0 -7.5px;
}
.circle span {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  transform: rotate(calc(18deg * var(--i)));
}
.circle span::before {
  content: "";
  position: absolute;
  right: 0;
  top: calc(50% - 7.5px);
  width: 15px;
  height: 15px;
  background: #317033;
  border-radius: 50%;
  box-shadow: 0 0 10px #317033,
   0 0 20px #317033,
   0 0 40px #317033,
   0 0 60px #317033;
   transform: scale(0.1);
   animation: breath 4s linear infinite;
   animation-delay: calc(0.1s * var(--i) );
}
@keyframes breath {
    0%{
        transform: scale(1);
    }
    50% , 100%{
        transform: scale(0.1);
    }
}
.circle:nth-child(2){
    transform: rotate(-180deg);
}
.circle:nth-child(2) span::before {
    animation-delay: calc(-0.1s * var(--i));
}
</style>