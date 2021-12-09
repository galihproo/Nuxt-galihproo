<template>
  <div>
    <Navbar />
    <div class="content">
      <Social />
      <div class="footer">
        <Footer />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
  @media (min-width: 992px) {
    .content {
      height: calc(100vh - 62px);
    }
    .footer {
      position: absolute;
      left: 0;
      bottom: 0;
      width: 100%;
    }
  }
</style>>