<script setup lang="ts">

</script>

<template>
  <div text-3xl>
    Test for anyway tab
    <a
      href="https://www.google.com"
      class="  href"
    >router</a>
  </div>
</template>

<style scoped>
  ::selection {
    background-color: #ffe324;
  }

  .href {
    position: relative;
  }

  .href:hover {
    background-color: #ffe324;
    transition: all 0s ease-in-out .7s;
  }

  .href::after  {
    background-color: #ffe324;
    display: block;
    content: "";
    height: 0%;
    z-index: -999;
    position: absolute;
    width: 100%;
    bottom: 0;
    left: 0;
  }

  .href:hover::after {
    /* transition: all .15s cubic-bezier(.8,0,.2,1); */
    animation: underline-in .7s cubic-bezier(.9,0,.1,1) 0s 1;
  }

  @keyframes underline-in {
    0% {
      height: 0;
    }

    0% {
      height: 0;
    }

    100% {
      height: 100%
    }
  }
</style>
