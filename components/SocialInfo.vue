<template>
  <ul class="social list-unstyled pt-1 mb-5">
    <li v-for="social in SocialShare" :key="social.id">
      <a :href="social.link" target="_blank" rel="noreferrer">
        <i :class="social.iconName"></i>
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      SocialShare: [
        {
          id: 1,
          iconName: "fa fa-github",
          link: "https://github.com/nomanhassan-coder",
        },
        {
          id: 2,
          iconName: "fa fa-linkedin",
          link: "https://www.linkedin.com/in/thenomanhassan/",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
