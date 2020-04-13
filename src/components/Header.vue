<template>
  <div class="header">
    <img alt="small-logo" src="../assets/logo3x.png"/>
  </div>
</template>

<style scoped lang="scss">
  @keyframes appear {
    0% {
      opacity: 0;
    }

    100% {
      opacity: 1;
    }
  }

  .header {
    opacity: 0;
    animation: 2s appear;
    animation-delay: 1s;
    animation-fill-mode: forwards;
    display: flex;
    width: 100%;
    padding-top: 30px;
    padding-bottom: 30px;
    height: auto;
    justify-content: center;
    align-items: center;

    img {
      width: 25%;
    }
  }
</style>
