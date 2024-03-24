<template>
  <div class="app-container">
    <p href="https://vuejs.org/" target="_blank">
      <h1 class="typing">Hello! My name is Andrea D'Auria</h1>
    </p>
  </div>
</template>


<script>
export default {
  name: 'App',
}
</script>

<style>
html, body {
  margin: 0;
  padding: 0;
  height: 100%;
  width: 100%;
  font-family: 'Roboto', sans-serif;
}

.app-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: #333; /* Dark grey background */
}

.typing {
  white-space: nowrap;
  overflow: hidden;
  border-right: .15em solid orange; /* Cursor like styling */
  animation: typing 4s steps(40, end), blink-caret .75s step-end infinite;
  color: white; /* Light color text for visibility on dark background */
}

/* Typing effect */
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

/* Cursor animations */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange; }
}
</style>
