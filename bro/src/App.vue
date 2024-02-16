<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam magnam ex amet laboriosam consequatur consectetur tempore tenetur. Eos ducimus iure alias et explicabo blanditiis iste reiciendis exercitationem voluptates libero? Obcaecati autem reprehenderit et ut quis eveniet! Repellendus quidem dolorem voluptatum obcaecati beatae aspernatur. Aperiam doloremque eaque, aspernatur quidem, enim officiis laboriosam itaque ad necessitatibus laborum quia tempora, deleniti non ratione animi unde voluptate quas provident excepturi laudantium ex voluptates iste. Dolorem qui atque ipsa ex animi repudiandae alias, repellendus fugiat amet ullam possimus natus quas optio tempore a consequuntur obcaecati magni cupiditate aliquid consectetur consequatur exercitationem. Omnis libero ea earum!</p>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
