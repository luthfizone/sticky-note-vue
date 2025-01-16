<script setup></script>

<template>
  <main>
    <div class="container">
      <!-- Header -->
      <header>
        <h1 class="header-title">Memo</h1>
        <button class="header-button">+</button>
      </header>

      <!-- Card -->
      <div class="card-container">
        <div class="card">
          <p class="card-content">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </p>
          <p class="card-date">12/12/2025</p>
        </div>
        <div class="card">
          <p class="card-content">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </p>
          <p class="card-date">12/12/2025</p>
        </div>
      </div>
    </div>

    <!-- Form overlay -->
    <div class="form-overlay">
      <div class="form-modal">
        <button class="form-close-btn">&times;</button>
        <textarea name="memo" id="memo" rows="10"></textarea>
        <button class="form-save-btn">save</button>
      </div>
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

/* card */
.card-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.card {
  width: 255px;
  height: 255px;
  padding: 10px;
  background-color: #ffa6c1;
  margin-bottom: 20px;

  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

/* form overlay */
.form-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.77);
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: center;
}

.form-modal {
  width: 420px;
  background-color: #fff;
  border-radius: 10px;
  padding: 30px;
  position: relative;
  display: flex;
  flex-direction: column;
}

.form-save-btn {
  background-color: #495a70;
  color: white;
  border: none;
  font-size: 20px;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  margin-top: 15px;
}

.form-save-btn:hover {
  background-color: #5e6e7f;
}

textarea {
  height: 200px;
  border-radius: 5px;
  font-family: Arial, Helvetica, sans-serif;
  padding: 10px;
  margin-bottom: 15px;
  outline: 1px solid #495a70;
}

textarea:focus {
  outline: 1px solid #495a70;
}

.form-close-btn {
  position: absolute;
  top: 5px;
  border: none;
  background-color: transparent;
  right: 10px;
  font-size: 25px;
  cursor: pointer;
}
</style>
