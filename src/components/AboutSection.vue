<template>
  <div class="background">
    <div class="container">
      <div>
        <img
          src="../assets/quem-somos.png"
          class="section-title"
        >
        <p class="content">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
          enim ad minim veniam, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
          pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
          culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <img
        src="../../public/placeholder.png"
        class="profile-picture"
      >
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 180px;
  height: 450px;
  gap: 100px;
}

.background {
  background-color: var(--blue);
}

.section-title {
  width: 300px;
}

.content {
  width: 600px;
  color: var(--white);
  font-size: 20px;
  line-height: 30px;
  text-align: justify;
}

.profile-picture {
  width: 300px;
  height: 400px;
  object-fit: cover;
  border-radius: 26px;
  margin-left: 50px;
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
    padding: 10px 20px;
    gap: 30px;
    height: auto;
  }

  .section-title {
    width: 100%;
    max-width: 250px;
    margin: 0 auto;
  }

  .content {
    width: 100%;
    max-width: 100%;
    font-size: 16px;
    line-height: 24px;
    text-align: justify;
  }

  .profile-picture {
    width: 80%;
    height: auto;
    max-width: 250px;
    margin: 0 auto;
  }
}

@media (max-width: 480px) {
  .content {
    font-size: 14px;
    line-height: 20px;
  }

  .profile-picture {
    max-width: 200px;
  }
}
</style>
