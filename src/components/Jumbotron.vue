<template>
    <div class="logo">
      <img src="../assets/logo3x.png" alt="logo">
    </div>
</template>

<style scoped lang="scss">
  @keyframes fade {
    0% {
      opacity: 1;
      visibility: visible;
    }

    100% {
      opacity: 0;
      visibility: hidden;
    }
  }

  .logo {
    position: absolute;
    animation: 2s fade;
    animation-fill-mode: forwards;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    width: 100%;
    background-color: #fff;
  }

  img {
    width: 40%;
  }
</style>
