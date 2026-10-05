<template>
  <ul>
    <li v-for="education in educationContent" :key="education.id">
      <div class="icon">
        <i class="fa fa-briefcase"></i>
      </div>
      <span class="time open-sans-font text-uppercase">{{
        education.year
      }}</span>
      <h5 class="poppins-font text-uppercase">
        {{ education.degree }}
        <span class="place open-sans-font">{{ education.institute }}</span>
      </h5>
      <p class="open-sans-font">{{ education.details }}</p>
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      educationContent: [
        {
          id: 1,
          year: "2023 - CONTINUE",
          degree: "BACHELOR DEGREE",
          institute: "UNIVERSITY OF SOUTH ASIA",
          details: `  Currently pursuing a Bachelor's degree in Software Engineering, with a growing focus on DevOps practices, cloud infrastructure, CI/CD pipelines, containerization, and system automation. Alongside my studies, I am actively working on hands-on projects to strengthen my understanding of deployment workflows, scalable systems, and modern DevOps tools and technologies.`,
        },
        {
          id: 2,
          year: "2020 - 2023",
          degree: "INTERMEDIATE",
          institute: "UNIQUE GROUP OF INSTITUTIONS",
          details: `Completed Intermediate studies in Pre-Engineering, developing a solid foundation in Mathematics, Physics, and analytical thinking. This academic background enhanced logical reasoning and prepared me for advanced studies in technology and engineering.`,
        },
        {
          id: 3,
          year: "2018 - 2020",
          degree: "MATRICULATION ",
          institute: "GOVERNMENT HIGH SCHOOL",
          details: `Completed Matriculation with Computer Science, where I developed an early interest in programming, computer fundamentals, and technology. This sparked my passion for software development and laid the groundwork for pursuing a career in Software Engineering.`,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
