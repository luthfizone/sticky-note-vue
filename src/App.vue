<script setup></script>

<template>
  <main>
    <div class="container">
      <!-- Header -->
      <header>
        <h1 class="header-title">Memo</h1>
        <button class="header-button">+</button>
      </header>
      <div>[card]</div>
    </div>
  </main>
</template>

<style scoped>
main {
  min-height: 100vh;
}

.container {
  max-width: 900px;
  padding: 10px;
  margin: 0 auto;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header-title {
  font-size: 48px;
  font-weight: bold;
  margin-bottom: 25px;
  color: #494040;
}

.header-button {
  border: none;
  padding: 5px;
  font-size: large;
  cursor: pointer;
  border-radius: 100%;
  color: white;
  background-color: #494040;
  width: 30px;
  height: 30px;
}

.header-button:hover {
  background-color: #5e5b5b;
}

.header-button:active {
  transform: scale(0.9);
  transition: transform 0.1s ease-in-out;
}
</style>
