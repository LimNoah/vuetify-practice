<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to Vuetifyy
        </h1>

        <p class="subheading font-weight-regular">
          For help and collaboration with other Vuetify developers,
          <br>please join our online
          <a
            href="https://community.vuetifyjs.com"
            target="_blank"
          >Discord Community</a>
        </p>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <div>
          <v-alert
            border="top"
            color="red lighten-2"
            dark
          >
            I'm an alert with a top border and red color
          </v-alert>
          <v-alert
            border="right"
            color="blue-grey"
            dark
          >
            I'm an alert with a right border and blue-grey color
          </v-alert>
          <v-alert
            border="bottom"
            color="pink darken-1"
            dark
          >
            I'm an alert with a bottom border and pink color
          </v-alert>
          <v-alert
            border="left"
            color="indigo"
            dark
          >
            I'm an alert with a border left type info
          </v-alert>
        </div>
        <div>
          <v-alert
            border="left"
            colored-border
            color="deep-purple accent-4"
            elevation="2"
          >
            Aliquam eu nunc. Fusce commodo aliquam arcu. In consectetuer turpis ut velit. Nulla facilisi..

            Morbi mollis tellus ac sapien. Fusce vel dui. Praesent ut ligula non mi varius sagittis. Vivamus consectetuer hendrerit lacus. Suspendisse enim turpis, dictum sed, iaculis a, condimentum nec, nisi.
          </v-alert>
          <v-alert
            border="top"
            colored-border
            type="info"
            elevation="2"
          >
            Vestibulum ullamcorper mauris at ligula. Nam pretium turpis et arcu. Ut varius tincidunt libero. Curabitur ligula sapien, tincidunt non, euismod vitae, posuere imperdiet, leo. Morbi nec metus.
          </v-alert>
          <v-alert
            border="bottom"
            colored-border
            type="warning"
            elevation="2"
          >
            Sed in libero ut nibh placerat accumsan. Phasellus leo dolor, tempus non, auctor et, hendrerit quis, nisi. Phasellus leo dolor, tempus non, auctor et, hendrerit quis, nisi. Sed consequat, leo eget bibendum sodales, augue velit cursus nunc, quis gravida magna mi a libero. Donec elit libero, sodales nec, volutpat a, suscipit non, turpis.
          </v-alert>
          <v-alert
            border="right"
            colored-border
            type="error"
            elevation="2"
          >
            Fusce commodo aliquam arcu. Pellentesque posuere. Phasellus tempus. Donec posuere vulputate arcu.
          </v-alert>
          <v-alert
              dense
              type="info"
            >
              I'm a dense alert with a <strong>type</strong> of info
            </v-alert>
            <v-alert
              dense
              text
              type="success"
            >
              I'm a dense alert with the <strong>text</strong> prop and a <strong>type</strong> of success
            </v-alert>
            <v-alert
              dense
              border="left"
              type="warning"
            >
              I'm a dense alert with the <strong>border</strong> prop and a <strong>type</strong> of warning
            </v-alert>
            <v-alert
              dense
              outlined
              type="error"
            >
              I'm a dense alert with the <strong>outlined</strong> prop and a <strong>type</strong> of error
            </v-alert>
            <div>
              <v-alert
                v-model="alert"
                border="left"
                close-text="Close Alert"
                color="deep-purple accent-4"
                dark
                dismissible
              >
                Aenean imperdiet. Quisque id odio. Cras dapibus. Pellentesque ut neque. Cras dapibus.

                Vivamus consectetuer hendrerit lacus. Sed mollis, eros et ultrices tempus, mauris ipsum aliquam libero, non adipiscing dolor urna a orci. Sed mollis, eros et ultrices tempus, mauris ipsum aliquam libero, non adipiscing dolor urna a orci. Curabitur blandit mollis lacus. Curabitur ligula sapien, tincidunt non, euismod vitae, posuere imperdiet, leo.
              </v-alert>
              <v-alert
                  color="#2A3B4D"
                  dark
                  icon="mdi-firework"
                  dense
                >
                  Suspendisse enim turpis, dictum sed, iaculis a, condimentum nec, nisi. Vivamus quis mi. Quisque ut nisi. Maecenas malesuada.
                </v-alert>
                <v-alert
                  color="#C51162"
                  dark
                  icon="mdi-material-design"
                  border="right"
                >
                  Phasellus blandit leo ut odio. Morbi mattis ullamcorper velit. Donec orci lectus, aliquam ut, faucibus non, euismod id, nulla. In ut quam vitae odio lacinia tincidunt.
                </v-alert>
                <v-alert
                  color="primary"
                  dark
                  icon="mdi-vuetify"
                  border="left"
                  prominent
                >
                  Praesent congue erat at massa. Nullam vel sem. Aliquam lorem ante, dapibus in, viverra quis, feugiat a, tellus. Proin viverra, ligula sit amet ultrices semper, ligula arcu tristique sapien, a accumsan nisi mauris ac eros. Curabitur at lacus ac velit ornare lobortis.
                </v-alert>
                <v-alert
                  outlined
                  color="purple"
                >
                  <div class="text-h6">
                    Lorem Ipsum
                  </div>
                  <div>Maecenas ullamcorper, dui et placerat feugiat, eros pede varius nisi, condimentum viverra felis nunc et lorem. Duis vel nibh at velit scelerisque suscipit. Praesent blandit laoreet nibh. Aenean posuere, tortor sed cursus feugiat, nunc augue blandit nunc, eu sollicitudin urna dolor sagittis lacus. Etiam sollicitudin, ipsum eu pulvinar rutrum, tellus ipsum laoreet sapien, quis venenatis ante odio sit amet eros.</div>
                </v-alert>
                <v-alert
                  outlined
                  type="success"
                  text
                >
                  Praesent venenatis metus at tortor pulvinar varius. Aenean commodo ligula eget dolor. Praesent ac massa at ligula laoreet iaculis. Vestibulum ullamcorper mauris at ligula.
                </v-alert>
                <v-alert
                  outlined
                  type="warning"
                  prominent
                  border="left"
                >
                  Duis arcu tortor, suscipit eget, imperdiet nec, imperdiet iaculis, ipsum. Suspendisse non nisl sit amet velit hendrerit rutrum. Nullam vel sem. Pellentesque dapibus hendrerit tortor.
                </v-alert>
                <v-alert
                  prominent
                  type="error"
                >
                  <v-row align="center">
                    <v-col class="grow">
                      Nunc nonummy metus. Nunc interdum lacus sit amet orci. Nullam dictum felis eu pede mollis pretium. Cras id dui.
                    </v-col>
                    <v-col class="shrink">
                      <v-btn>Take action</v-btn>
                    </v-col>
                  </v-row>
                </v-alert>
                <v-alert
                  color="blue-grey"
                  dark
                  dense
                  icon="mdi-school"
                  prominent
                >
                  Sed augue ipsum, egestas nec, vestibulum et, malesuada adipiscing, dui. Aenean ut eros et nisl sagittis vestibulum. Sed aliquam ultrices mauris. Donec vitae orci sed dolor rutrum auctor.
                </v-alert>
                <v-alert
                  icon="mdi-shield-lock-outline"
                  prominent
                  text
                  type="info"
                >
                  Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Sed in libero ut nibh placerat accumsan.. Curabitur blandit mollis lacus. Curabitur blandit mollis lacus.
                </v-alert>
                <v-alert type="success">
                  I'm a success alert.
                </v-alert>

                <v-alert type="info">
                  I'm an info alert.
                </v-alert>

                <v-alert type="warning">
                  I'm a warning alert.
                </v-alert>

                <v-alert type="error">
                  I'm an error alert.
                </v-alert>
                <v-alert
                  v-model="alert"
                  dismissible
                  color="cyan"
                  border="left"
                  elevation="2"
                  colored-border
                  icon="mdi-twitter"
                >
                  You've got <strong>5</strong> new updates on your timeline!.
                </v-alert>

                <div class="text-center">
                  <v-btn
                    v-if="!alert"
                    dark
                    @click="alert = true"
                  >
                    Reset Alert
                  </v-btn>
                </div>
              <div class="text-center">
                <v-btn
                  v-if="!alert"
                  color="deep-purple accent-4"
                  dark
                  @click="alert = true"
                >
                  Reset
                </v-btn>
              </div>
            </div>
        </div>
        <v-bottom-navigation v-model="value">
          <v-btn value="recent">
            <span>Recent</span>

            <v-icon>mdi-history</v-icon>
          </v-btn>

          <v-btn value="favorites">
            <span>Favorites</span>

            <v-icon>mdi-heart</v-icon>
          </v-btn>

          <v-btn value="nearby">
            <span>Nearby</span>

            <v-icon>mdi-map-marker</v-icon>
          </v-btn>
        </v-bottom-navigation>
        <v-bottom-navigation
          :value="value"
          color="teal"
          grow
        >
          <v-btn>
            <span>Recents</span>

            <v-icon>mdi-history</v-icon>
          </v-btn>

          <v-btn>
            <span>Favorites</span>

            <v-icon>mdi-heart</v-icon>
          </v-btn>

          <v-btn>
            <span>Nearby</span>

            <v-icon>mdi-map-marker</v-icon>
          </v-btn>
        </v-bottom-navigation>
      </v-col>
      
      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          What's next?
        </h2>

        <v-row justify="center">
          <a
            v-for="(next, i) in whatsNext"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </a>
        </v-row>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          Important Links
        </h2>

        <v-row justify="center">
          <a
            v-for="(link, i) in importantLinks"
            :key="i"
            :href="link.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ link.text }}
          </a>
        </v-row>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          Ecosystem
        </h2>

        <v-row justify="center">
          <a
            v-for="(eco, i) in ecosystem"
            :key="i"
            :href="eco.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ eco.text }}
          </a>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'Select a layout',
          href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
        },
        {
          text: 'Frequently Asked Questions',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
  }
</script>
