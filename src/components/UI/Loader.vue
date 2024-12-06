<template>
  <div class="loader">
    <div class="spinner"></div>
  </div>
</template>

<style scoped>
.loader {
  position: fixed;
  top: 0;
  left: 0;
  width: 95vw;
  height: 100vh;
  background-color: rgb(0, 0, 0);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 999;
}

.spinner {
  border: 8px solid rgba(255, 255, 255, 0.3);
  border-top: 8px solid #ffffff; 
  border-radius: 50%;
  width: 50px;
  height: 50px;
  animation: spin 1s linear infinite; 
}

@keyframes spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}
</style>