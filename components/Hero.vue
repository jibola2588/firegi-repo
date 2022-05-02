<!-- Please remove this file from your project -->
<template>
  <div class="Hero">
    <div class="text-container">
      <h1 class="header">Find your Fire Extinguisher</h1>
    <p class="snippet">
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic nostrum
      ipsam maxime repudiandae assumenda consectetur amet inventore et ad,
      dolorum error, ab, tempore porro enim delectus tenetur iste optio impedit.
    </p>
    <button class="button btn">Start Looking</button>
    </div>
    <div>
      <img src="~assets/svg/fire-extinguisher.svg" alt="" class="image">
    </div>
  </div>
</template>

<script>
export default {
  name: 'NuxtHero',
}
</script>
<style scoped>
.Hero {
  /* height: 50vh; */
   margin-top: 4rem;
  position: relative;
  display: flex;
  flex-flow: row wrap;
  padding: 2rem;
  align-items: flex-start;
  justify-content: space-between;
}
.text-container {
  width: 50%;
  margin-top: 1rem;
}
.header {
  font-weight: 900;
  font-size: 4.3rem;
}
.snippet {
  color: grey;
  margin: 0.5rem 0;
  font-size: 1.05rem;
}
.image {
  /* width: 27.5rem; */
  width: 20.5rem;
  margin-top: 3rem;
}
.overlay {
  background: rgba(0, 0, 0, 0);
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
}
.button {
  margin-top: 0.9rem;
  padding: 1rem 4rem;
  border-radius: 100rem;
  background-color: rgb(231, 81, 43);
  color: white;
  width: 20rem;
  font-weight: 700;
  transition: 0.5s;
}
.button:hover {
  width: 21.5rem;
}
@media (max-width: 1024px) { 
  .header {
  font-weight: 900;
  font-size: 2.3rem;
}
}
@media (max-width: 500px) {
  .Hero {
    height: 40vh;
  }
}
</style>
