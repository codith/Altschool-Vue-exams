<template>
  <nav>
    <div class="counter-logo">Counter App</div>
    <div class="nav-links">
      <router-link to="/">Home</router-link>
      <router-link to="/counter">Counter</router-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style>
nav {
  display:flex;
  justify-content:space-between;
  align-items:center;
  background-color: rgb(110, 102, 102);
  color: inherit;
  border: none;
  width: 100%;
  padding: 14px;
  margin: 0 auto;
  box-shadow: 1px 1px 3px #555;
}

.counter-logo{
font-size: 2.4rem;
font-family: secFont;
font-weight: light;
letter-spacing: 2px;
margin-right: 15px;
}


.nav-links {
display: flex;
gap: 10px;
justify-content: space-between;
align-items: center;
font-family: 'Times New Roman';
margin-right: 15px;
}
.nav-links a {
font-size: 1.2rem;
color: white;
text-decoration:none;
margin-right: 1rem;
font-weight: bolder;
}

</style>
