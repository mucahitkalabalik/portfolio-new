<template>
  <section class="menu">

    <ul class="mt-15">
      <li style="--clr: #00ade1"><a href="#" data-text="Home">Home</a></li>
      <li style="--clr: #ff994b"><a href="#" data-text="About">About</a></li>
      <li style="--clr: #6eff60">
        <a href="#" data-text="Services">Services</a>
      </li>
      <li style="--clr: #ff60ff"><a href="#" data-text="Team">Team</a></li>
      <li style="--clr: #dc0000">
        <a href="#" data-text="Contact">Contact</a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.menu {
  margin-top: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 50vh;
  flex-direction: column;
}

ul {
  position: relative;
  display: flex;
  flex-direction: column;
  gap: 30px;
}
ul li {
  position: relative;
  list-style: none;
}
ul li a {
  position: relative;
  font-size: 4em;
  text-decoration: none;
  line-height: 1em;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: transparent;
  -webkit-text-stroke: 1px rgb(146, 143, 143);
}
ul li a::before {
  content: attr(data-text);
  position: absolute;
  color: var(--clr);
  width: 0%;
  overflow: hidden;
  transition: 1s;
  border-right: 8px solid var(--clr);
}
ul li a:hover::before {
  width: 100%;
  -webkit-text-stroke: 1px var(--clr);
}
</style>