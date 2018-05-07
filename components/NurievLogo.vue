<template>
  <img flex class="NurievLogo" alt="NurievLogo" src="~/static/foto51.png" width="100px">
</template>

<style>
  .NurievLogo {
    width: 360px;
    transform: rotateY(360deg);
    animation: turn 3.5s ease-out forwards 1s;
  }
  @keyframes turn {
    100% {
      transform: rotateY(0deg);
    }
  }
</style>
