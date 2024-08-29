<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>




<template>
  <head>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
  </head>

  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Jeugdhuis Volle Petrol heet u welkom
      <div class="socials">
        <a href="https://www.instagram.com/jeugdhuis_hechtel/" target="_blank" rel="noopener">
          <i class="fab fa-instagram"></i>
        </a>
        <a href="https://www.facebook.com/profile.php?id=61564316186457" target="_blank" rel="noopener">
          <i class="fab fa-facebook"></i>
        </a>
      </div>
    </h3>
  </div>
</template>


<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h3 .socials{
  font-size: 1.2rem;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
