<template>
  <div
    class="col-6 col-md-3 mb-3 mb-sm-5"
    :key="skills.id"
    v-for="skills in skillsContent"
  >
    <div :class="`c100 ${skills.skillClass}`">
      <span>{{ skills.skillPercent }}%</span>
      <div class="slice">
        <div class="bar"></div>
        <div class="fill"></div>
      </div>
    </div>
    <h6 class="text-uppercase open-sans-font text-center mt-2 mt-sm-4">
      {{ skills.skillName }}
    </h6>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skillsContent: [
        { 
          id: 1, 
          skillClass: "p90", 
          skillPercent: "90", 
          skillName: "AWS Cloud" 
        },
        {
          id: 2,
          skillClass: "p90",
          skillPercent: "90",
          skillName: "Docker",
        },
        { 
          id: 3, 
          skillClass: "p88", 
          skillPercent: "88", 
          skillName: "GitHub Actions" 
        },
        { 
          id: 4, 
          skillClass: "p88", 
          skillPercent: "88", 
          skillName: "Git & GitHub" 
        },
        {
          id: 5,
          skillClass: "p88",
          skillPercent: "88",
          skillName: "CI/CD Pipelines",
        },
        { 
          id: 6, 
          skillClass: "p90", 
          skillPercent: "90", 
          skillName: "Linux & Bash"
         },
        { 
          id: 7, 
          skillClass: "p70", 
          skillPercent: "70", 
          skillName: "Amazon EKS" 
        },
        { 
          id: 8, 
          skillClass: "p60", 
          skillPercent: "60", 
          skillName: "CloudFormation" 
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
