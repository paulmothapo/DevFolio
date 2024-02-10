<template>
  <NuxtLayout>
    <div>
      <div class="mouse-pointer"></div>
      <NuxtPage />
    </div>
  </NuxtLayout>
</template>

<script>
export default {
  mounted() {
    document.addEventListener('mousemove', this.handleMouseMove);
  },
  methods: {
    handleMouseMove(event) {
      const mouseX = event.clientX;
      const mouseY = event.clientY;
      const mousePointer = document.querySelector('.mouse-pointer');
      mousePointer.style.transform = `translate(${mouseX}px, ${mouseY}px)`;
    }
  },
  beforeDestroy() {
    document.removeEventListener('mousemove', this.handleMouseMove);
  }
}
</script>

<style>
.mouse-pointer {
  position: absolute;
  top: 0;
  left: 0;
  width: 40px;
  height: 40px;
  background-color: transparent;
  border: 2px solid #d20000;
  border-radius: 50%;
  mix-blend-mode: difference;
  pointer-events: none;
  transition: transform 0.2s ease;
  z-index: 9999;
}
</style>
