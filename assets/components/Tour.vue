<template>
  <v-tour name="dozzleTour" :steps="steps"></v-tour>
</template>

<script>
export default {
  name: "tour",
  data() {
    return {
      steps: [
        {
          target: "#hide-nav",
          header: {
            title: "Get Started",
          },
          content: `Discover <strong>Vue Tour</strong>!`,
        },
      ],
    };
  },
  mounted: function () {
    this.$tours["dozzleTour"].start();
  },
};
</script>
