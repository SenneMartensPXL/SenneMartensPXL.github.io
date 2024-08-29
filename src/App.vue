<script setup>
import { ref } from 'vue'
import { RouterLink, RouterView } from 'vue-router'

// Assume a state to check if the user is logged in
const loggedIn = ref(false)
const admin = ref(false)
</script>

<template>
  <header>
    <div class="topsec">
      <!-- Centered Logo -->
      <img alt="Volle Petrol logo" class="logo" src="@/assets/JeugdhuisVPTijdelijk-removebg-preview.png" width="125" height="125" />

      <!-- Profile or Login button depending on the state -->
      <div class="top-right">
        <div v-if="loggedIn" class="profile">
          <img alt="pfp" class="profile-pic" src="@/assets/JeugdhuisVPTijdelijk-removebg-preview.png" width="50" height="50" />
          <label id="username">Username</label>
        </div>
        <RouterLink v-else class="button" to="/login">Login</RouterLink>
      </div>
    </div>

    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/events">Events</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/team">Our team</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
        <RouterLink to="/Join">Join our team</RouterLink>
        <RouterLink v-if="admin" to="/adminPanel">AdminPanel</RouterLink>
      </nav>
    </div>

    <!--HelloWorld msg="Welkom"/-->
  </header>

  <RouterView />
</template>

<style scoped>

body {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.topsec{
  display: flex;
  justify-content: center;
  position: relative;
  width: 100%;
}

.logo {
  margin: auto;
}

.top-right {
  position: absolute;
  top: 0;
  right: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.profile{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

header {
  line-height: 1.5;
  max-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 1rem;
}

nav {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1.5rem;
}

nav a {
  font-size: 1rem;
  text-decoration: none;
  color: var(--color-text);
  padding: 0.5rem 1rem;
  transition: color 0.3s ease, background-color 0.3s ease;
}

nav a.router-link-exact-active {
  color: var(--color-heading);
}

nav a:hover {
  color: var(--color-border-hover);
}

.button {
  font-size: 1rem;
  text-decoration: none;
  color: var(--color-text);
  padding: 0.5rem 1rem;
  transition: color 0.3s ease, background-color 0.3s ease;
}

.button.router-link-exact-active {
  color: var(--color-heading);
}

.button:hover {
  color: var(--color-border-hover);
}

@media (min-width: 1024px) {
  header {
    justify-content: space-between;
    padding: 1rem 2rem;
  }

  .logo {
    margin: 0;
  }

  .wrapper {
    display: flex;
    align-items: center;
    padding: 20px;
  }
}
</style>
