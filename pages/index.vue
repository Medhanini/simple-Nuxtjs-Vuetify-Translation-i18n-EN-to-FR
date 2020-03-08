<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-center">
        Made with Love BY MedHAnini
      </div>
      <v-card>
        <v-card-title class="headline">
                {{ $t('home.title') }}
        </v-card-title>
        <v-card-text>
            <div class="Content">
            <div class="container">
              <p>{{ $t('home.introduction') }}</p>
            </div>
          </div>
          <div class="text-xs-right">
            <em><small>&mdash; MedHanini</small></em>
          </div>
          <hr class="my-3">
          <a
            href="https://www.linkedin.com/in/mohamed-hanini-580a16166/"
            target="_blank"
          >
            linkedin
          </a>
          <br>
          <a
            href="https://github.com/Medhanini"
            target="_blank"
          >
            GitHub
          </a>
        </v-card-text>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  },
    head () {
    return { title: this.$t('home.title') }
  }
}
</script>
