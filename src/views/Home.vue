<template>
  <v-app>
    <v-container
      align="center"
      class="home bg-image fill-height  d-flex flex-column justify-content-center"
      fluid
      id="home"
    >
      <v-row :justify="'center'" :align="'center'">
        <v-col cols="12" class="text-center">
          <img src="/img/illustrations/conversation.svg" alt="Cloud therapy home background" id="bgHome"/>
          <h1>It's okay not to be okay</h1>
          <h4>
            A safe space to share with peers anonymously
          </h4>
          <v-btn to="/auth" class="ct-shadow mt-5 btn-cta" color="primary" x-large>
            Get Started
          </v-btn>
        </v-col>
      </v-row>
    </v-container>

    <SiteFooter />
  </v-app>
</template>

<script>
import SiteFooter from '@/components/templates/SiteFooter';

export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Home",
  components: {
    SiteFooter
  },
  created() {
    document.title = "Cloudtherapy - It's okay not to be okay";
  }
};
</script>

<style scoped lang="scss">
  h1{
    line-height: 120%;
    margin-bottom: 1rem;
  }
  #bgHome {
    width: 120%;
    min-width:18rem;
    max-width: 45rem;
    max-height: 50vh;
  }

  .btn-cta{
    width: 100%;
    margin: auto;
    max-width:24rem;
    height: 3.6rem;
    border-radius: 3rem !important;
  }
</style>