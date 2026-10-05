<template>
  <ul class="about-list list-unstyled open-sans-font">
    <li v-for="personalInfo in personalInfoContent" :key="personalInfo.id">
      <span class="title">{{ personalInfo.meta }}: </span>
      <span
        class="value d-block d-sm-inline-block d-lg-block d-xl-inline-block"
      >
        {{ personalInfo.metaInfo }}
      </span>
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      personalInfoContent: [
        { id: 1, meta: "first name", metaInfo: "Noman" },
        { id: 2, meta: "last name", metaInfo: "Hassan" },
        { id: 3, meta: "Age", metaInfo: "20 Years" },
        { id: 4, meta: "Nationality", metaInfo: "Pakistani" },
        { id: 5, meta: "Freelance", metaInfo: "Available" },
        { id: 6, meta: "Address", metaInfo: "Lahore" },
        { id: 7, meta: "phone", metaInfo: "+923245454100" },
        { id: 8, meta: "Email", metaInfo: "mr9miofficial@gmail.com" },
        { id: 10, meta: "langages", metaInfo: "English, Urdu" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
