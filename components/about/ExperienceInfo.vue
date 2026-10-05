<template>
  <ul>
    <li v-for="experience in experienceContent" :key="experience.id">
      <div class="icon">
        <i class="fa fa-briefcase"></i>
      </div>
      <span class="time open-sans-font text-uppercase">{{
        experience.year
      }}</span>
      <h5 class="poppins-font text-uppercase">
        {{ experience.position }}
        <span class="place open-sans-font">{{ experience.compnayName }}</span>
      </h5>
      <p class="open-sans-font">{{ experience.details }}</p>
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      experienceContent: [
        {
          id: 1,
          year: "   2015 - 2026",
          position: " DevOps Intern",
          compnayName: "RTC League",
          details: `  Working as a DevOps Intern, gaining practical experience with CI/CD pipelines, Docker, Linux, cloud services, and deployment automation. Collaborating with the development team to streamline software delivery, improve infrastructure reliability, and implement modern DevOps best practices.`,
        },
        {
          id: 2,
          year: "2024 ( 6 months )",
          position: " Web Developer Intern",
          compnayName: "Royal Monarch Industries",
          details: `Completed a six-month internship as a Web Developer, where I contributed to the development and maintenance of responsive web applications. Worked with modern web technologies, collaborated with senior developers, fixed bugs, implemented new features, and gained hands-on experience in building user-friendly and scalable web solutions.`,
        },
        // {
        //   id: 3,
        //   year: "2005 - 2013",
        //   position: "Consultant",
        //   compnayName: "Videohive",
        //   details: `Lorem ipsum dolor sit amet, tempor incididunt ut laboreconsectetur
        // elit, sed do eiusmod tempor duntt`,
        // },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
