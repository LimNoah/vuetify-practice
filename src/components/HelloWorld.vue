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
        <v-card
          class="overflow-hidden mx-auto"
          height="200"
          max-width="500"
        >
          <v-bottom-navigation
            absolute
            hide-on-scroll
            horizontal
            scroll-target="#hide-on-scroll-example"
          >
            <v-btn
              color="deep-purple accent-4"
              text
            >
              <span>Recents</span>

              <v-icon>mdi-history</v-icon>
            </v-btn>

            <v-btn
              color="deep-purple accent-4"
              text
            >
              <span>Favorites</span>

              <v-icon>mdi-heart</v-icon>
            </v-btn>

            <v-btn
              color="deep-purple accent-4"
              text
            >
              <span>Nearby</span>

              <v-icon>mdi-map-marker</v-icon>
            </v-btn>
          </v-bottom-navigation>

          <v-responsive
            id="hide-on-scroll-example"
            class="overflow-y-auto"
            max-height="600"
          >
            <v-responsive height="1500"></v-responsive>
          </v-responsive>
        </v-card>
        <v-card
          class="mx-auto overflow-hidden"
          height="200"
          max-width="500"
        >
          <v-bottom-navigation
            absolute
            color="white"
            hide-on-scroll
            horizontal
            scroll-target="#scroll-threshold-example"
            scroll-threshold="500"
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

          <v-sheet
            id="scroll-threshold-example"
            class="overflow-y-auto pb-16"
            max-height="600"
          >
            <v-responsive height="1500"></v-responsive>
          </v-sheet>
        </v-card>
        <v-bottom-navigation
          v-model="value"
          :background-color="color"
          dark
          shift
        >
          <v-btn>
            <span>Video</span>

            <v-icon>mdi-television-play</v-icon>
          </v-btn>

          <v-btn>
            <span>Music</span>

            <v-icon>mdi-music-note</v-icon>
          </v-btn>

          <v-btn>
            <span>Book</span>

            <v-icon>mdi-book</v-icon>
          </v-btn>

          <v-btn>
            <span>Image</span>

            <v-icon>mdi-image</v-icon>
          </v-btn>
        </v-bottom-navigation>
        <div class="overflow-hidden">
          <div class="text-center mb-8">
            <v-btn
              color="deep-purple"
              outlined
              @click="active = !active"
            >
              Toggle Navigation
            </v-btn>
          </div>

          <v-bottom-navigation
            v-model="value"
            :input-value="active"
            color="indigo"
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
        </div>
        <v-bottom-sheet
          v-model="sheet"
          inset
        >
          <template v-slot:activator="{ on, attrs }">
            <v-btn
              color="orange"
              dark
              v-bind="attrs"
              v-on="on"
            >
              Open Inset
            </v-btn>
          </template>
          <v-sheet
            class="text-center"
            height="200px"
          >
            <v-btn
              class="mt-6"
              text
              color="error"
              @click="sheet = !sheet"
            >
              close
            </v-btn>
            <div class="my-3">
              This is a bottom sheet using the inset prop
            </div>
          </v-sheet>
        </v-bottom-sheet>
        <v-btn
          color="blue"
          dark
          @click="sheet = !sheet"
        >
          Open v-model
        </v-btn>
        <v-bottom-sheet v-model="sheet">
          <v-sheet
            class="text-center"
            height="200px"
          >
            <v-btn
              class="mt-6"
              text
              color="red"
              @click="sheet = !sheet"
            >
              close
            </v-btn>
            <div class="py-3">
              This is a bottom sheet using the controlled by v-model instead of activator
            </div>
          </v-sheet>
        </v-bottom-sheet>
        <div class="text-center">
          <v-bottom-sheet
            v-model="sheet"
            persistent
          >
            <template v-slot:activator="{ on, attrs }">
              <v-btn
                color="green"
                dark
                v-bind="attrs"
                v-on="on"
              >
                Open Persistent
              </v-btn>
            </template>
            <v-sheet
              class="text-center"
              height="200px"
            >
              <v-btn
                class="mt-6"
                text
                color="error"
                @click="sheet = !sheet"
              >
                close
              </v-btn>
              <div class="py-3">
                This is a bottom sheet using the persistent prop
              </div>
            </v-sheet>
          </v-bottom-sheet>
        </div>
        <div class="text-center">
          <v-bottom-sheet inset>
            <template v-slot:activator="{ on, attrs }">
              <v-btn
                color="red"
                dark
                v-bind="attrs"
                v-on="on"
              >
                Open Player
              </v-btn>
            </template>
            <v-card tile>
              <v-progress-linear
                :value="50"
                class="my-0"
                height="3"
              ></v-progress-linear>

              <v-list>
                <v-list-item>
                  <v-list-item-content>
                    <v-list-item-title>The Walker</v-list-item-title>
                    <v-list-item-subtitle>Fitz & The Trantrums</v-list-item-subtitle>
                  </v-list-item-content>

                  <v-spacer></v-spacer>

                  <v-list-item-icon>
                    <v-btn icon>
                      <v-icon>mdi-rewind</v-icon>
                    </v-btn>
                  </v-list-item-icon>

                  <v-list-item-icon :class="{ 'mx-5': $vuetify.breakpoint.mdAndUp }">
                    <v-btn icon>
                      <v-icon>mdi-pause</v-icon>
                    </v-btn>
                  </v-list-item-icon>

                  <v-list-item-icon
                    class="ml-0"
                    :class="{ 'mr-3': $vuetify.breakpoint.mdAndUp }"
                  >
                    <v-btn icon>
                      <v-icon>mdi-fast-forward</v-icon>
                    </v-btn>
                  </v-list-item-icon>
                </v-list-item>
              </v-list>
            </v-card>
          </v-bottom-sheet>
        </div>
        <div class="text-center">
          <v-bottom-sheet v-model="sheet">
            <template v-slot:activator="{ on, attrs }">
              <v-btn
                color="purple"
                dark
                v-bind="attrs"
                v-on="on"
              >
                Open In
              </v-btn>
            </template>
            <v-list>
              <v-subheader>Open in</v-subheader>
              <v-list-item
                v-for="tile in tiles"
                :key="tile.title"
                @click="sheet = false"
              >
                <v-list-item-avatar>
                  <v-avatar
                    size="32px"
                    tile
                  >
                    <img
                      :src="`https://cdn.vuetifyjs.com/images/bottom-sheets/${tile.img}`"
                      :alt="tile.title"
                    >
                  </v-avatar>
                </v-list-item-avatar>
                <v-list-item-title>{{ tile.title }}</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-bottom-sheet>
        </div>
        <div class="text-center">
          <v-btn block>
            Block Button
          </v-btn>
        </div>
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
      <v-col
        cols="12"
        md="4"
      >
        <v-text-field
          v-model="firstname"
          :rules="nameRules"
          :counter="10"
          label="First name"
          required
        ></v-text-field>
      </v-col>

      <v-col
        cols="12"
        md="4"
      >
        <v-text-field
          v-model="lastname"
          :rules="nameRules"
          :counter="10"
          label="Last name"
          required
        ></v-text-field>
      </v-col>

      <v-col
        cols="12"
        md="4"
      >
        <v-text-field
          v-model="email"
          :rules="emailRules"
          label="E-mail"
          required
        ></v-text-field>
      </v-col>
    </v-row>
    <v-row
      justify="space-between"
    >
      <v-col
        cols="12"
        md="4"
      >
        <v-form ref="form">
          <v-text-field
            v-model="model"
            :counter="max"
            :rules="rules"
            label="First name"
          ></v-text-field>
        </v-form>
      </v-col>

      <v-col
        cols="12"
        md="6"
      >
        <v-slider
          v-model="max"
          label="Max characters"
        >
        </v-slider>

        <v-checkbox
          v-model="allowSpaces"
          label="Allow spaces"
        ></v-checkbox>

        <v-text-field
          v-model="match"
          label="Value must match"
        ></v-text-field>
      </v-col>
    </v-row>
    <v-form
      ref="form"
      v-model="valid"
      lazy-validation
    >
      <v-text-field
        v-model="name"
        :counter="10"
        :rules="nameRules"
        label="Name"
        required
      ></v-text-field>

      <v-text-field
        v-model="email"
        :rules="emailRules"
        label="E-mail"
        required
      ></v-text-field>

      <v-select
        v-model="select"
        :items="items"
        :rules="[v => !!v || 'Item is required']"
        label="Item"
        required
      ></v-select>

      <v-checkbox
        v-model="checkbox"
        :rules="[v => !!v || 'You must agree to continue!']"
        label="Do you agree?"
        required
      ></v-checkbox>

      <v-btn
        :disabled="!valid"
        color="success"
        class="mr-4"
        @click="validate"
      >
        Validate
      </v-btn>

      <v-btn
        color="error"
        class="mr-4"
        @click="reset"
      >
        Reset Form
      </v-btn>

      <v-btn
        color="warning"
        @click="resetValidation"
      >
        Reset Validation
      </v-btn>
    </v-form>
    <v-row>
      <v-col cols="12">
        <v-input
          :messages="['Messages']"
          append-icon="mdi-close"
          prepend-icon="mdi-phone"
        >
          Default Slot
        </v-input>
      </v-col>
    </v-row>
    <div>
      <v-text-field
        label="Main input"
        :rules="rules"
        hide-details="auto"
      ></v-text-field>
      <v-text-field label="Another input"></v-text-field>
    </div>
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
