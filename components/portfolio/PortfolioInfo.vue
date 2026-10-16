<template>
  <div class="portfolio-main">
    <div class="container">
      <div class="portfolio-coming-soon" role="status">
        <h2>Coming Soon</h2>
        <p>New projects are currently being prepared.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FancyPortfolio",
};
</script>

<style lang="scss" scoped>
.portfolio-coming-soon {
  align-items: center;
  border: 1px solid rgba(255, 180, 0, 0.35);
  border-radius: 0.5rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0 auto;
  max-width: 720px;
  min-height: 260px;
  padding: 40px 20px;
  text-align: center;

  h2 {
    color: var(--main-primary-color);
    font-size: 36px;
    margin-bottom: 12px;
    text-transform: uppercase;
  }

  p {
    margin: 0;
  }
}

:global(body.light) .portfolio-coming-soon {
  border-color: rgba(255, 180, 0, 0.6);
}
</style>
