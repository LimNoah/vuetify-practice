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
    <v-row>
      <v-switch
        v-model="showMessages"
        label="Show messages"
      ></v-switch>
      <v-input
        hint="I am hint"
        persistent-hint
        :messages="messages"
      >
        Input
      </v-input>
    </v-row>
    <v-text-field
      color="success"
      loading
      disabled
    ></v-text-field>
    <v-input
      :success-messages="['Success']"
      success
      disabled
    >
      Input
    </v-input>
    <div>
      <v-sheet
        tile
        height="54"
        class="d-flex"
      >
        <v-btn
          icon
          class="ma-2"
          @click="$refs.calendar.prev()"
        >
          <v-icon>mdi-chevron-left</v-icon>
        </v-btn>
        <v-select
          v-model="type"
          :items="types"
          dense
          outlined
          hide-details
          class="ma-2"
          label="type"
        ></v-select>
        <v-select
          v-model="mode"
          :items="modes"
          dense
          outlined
          hide-details
          label="event-overlap-mode"
          class="ma-2"
        ></v-select>
        <v-select
          v-model="weekday"
          :items="weekdays"
          dense
          outlined
          hide-details
          label="weekdays"
          class="ma-2"
        ></v-select>
        <v-spacer></v-spacer>
        <v-btn
          icon
          class="ma-2"
          @click="$refs.calendar.next()"
        >
          <v-icon>mdi-chevron-right</v-icon>
        </v-btn>
      </v-sheet>
      <v-sheet height="600">
        <v-calendar
          ref="calendar"
          v-model="value"
          :weekdays="weekday"
          :type="type"
          :events="events"
          :event-overlap-mode="mode"
          :event-overlap-threshold="30"
          :event-color="getEventColor"
          @change="getEvents"
        ></v-calendar>
      </v-sheet>
    </div>
    <v-row class="fill-height">
      <v-col>
        <v-sheet height="64">
          <v-toolbar
            flat
          >
            <v-btn
              outlined
              class="mr-4"
              color="grey darken-2"
              @click="setToday"
            >
              Today
            </v-btn>
            <v-btn
              fab
              text
              small
              color="grey darken-2"
              @click="prev"
            >
              <v-icon small>
                mdi-chevron-left
              </v-icon>
            </v-btn>
            <v-btn
              fab
              text
              small
              color="grey darken-2"
              @click="next"
            >
              <v-icon small>
                mdi-chevron-right
              </v-icon>
            </v-btn>
            <v-toolbar-title v-if="$refs.calendar">
              {{ $refs.calendar.title }}
            </v-toolbar-title>
            <v-spacer></v-spacer>
          </v-toolbar>
        </v-sheet>
        <v-sheet height="600">
          <v-calendar
            ref="calendar"
            v-model="focus"
            color="primary"
            type="category"
            category-show-all
            :categories="categories"
            :events="events"
            :event-color="getEventColor"
            @change="fetchEvents"
          ></v-calendar>
        </v-sheet>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-sheet height="400">
          <v-calendar
            ref="calendar"
            :now="today"
            :value="today"
            :events="events"
            color="primary"
            type="week"
          ></v-calendar>
        </v-sheet>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-sheet height="500">
          <v-calendar
            :now="today"
            :value="today"
            color="primary"
          >
            <template v-slot:day="{ past, date }">
              <v-row
                class="fill-height"
              >
                <template v-if="past && tracked[date]">
                  <v-sheet
                    v-for="(percent, i) in tracked[date]"
                    :key="i"
                    :title="category[i]"
                    :color="colors[i]"
                    :width="`${percent}%`"
                    height="100%"
                    tile
                  ></v-sheet>
                </template>
              </v-row>
            </template>
          </v-calendar>
        </v-sheet>
      </v-col>
    </v-row>

    <v-row>
      <v-col>
        <v-sheet height="500">
          <v-calendar
            ref="calendar"
            v-model="value"
            type="week"
          >
            <template v-slot:day-body="{ date, week }">
              <div
                class="v-current-time"
                :class="{ first: date === week[0].date }"
                :style="{ top: nowY }"
              ></div>
            </template>
          </v-calendar>
        </v-sheet>
      </v-col>
    </v-row>
    <v-row class="fill-height">
      <v-col>
        <v-sheet height="600">
          <v-calendar
            ref="calendar"
            v-model="value"
            color="primary"
            type="4day"
            :events="events"
            :event-color="getEventColor"
            :event-ripple="false"
            @change="getEvents"
            @mousedown:event="startDrag"
            @mousedown:time="startTime"
            @mousemove:time="mouseMove"
            @mouseup:time="endDrag"
            @mouseleave.native="cancelDrag"
          >
            <template v-slot:event="{ event, timed, eventSummary }">
              <div class="v-event-draggable">
                <component :is="{ render: eventSummary }"></component>
              </div>
              <div
                v-if="timed"
                class="v-event-drag-bottom"
                @mousedown.stop="extendBottom(event)"
              ></div>
            </template>
          </v-calendar>
        </v-sheet>
      </v-col>
    </v-row>
    <v-divider></v-divider>
    <v-card
    :loading="loading"
    class="mx-auto my-12"
    max-width="374"
  >
    <template slot="progress">
      <v-progress-linear
        color="deep-purple"
        height="10"
        indeterminate
      ></v-progress-linear>
    </template>

    <v-img
      height="250"
      src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
    ></v-img>

    <v-card-title>Cafe Badilico</v-card-title>

    <v-card-text>
      <v-row
        align="center"
        class="mx-0"
      >
        <v-rating
          :value="4.5"
          color="amber"
          dense
          half-increments
          readonly
          size="14"
        ></v-rating>

        <div class="grey--text ms-4">
          4.5 (413)
        </div>
      </v-row>

      <div class="my-4 text-subtitle-1">
        $ • Italian, Cafe
      </div>

      <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
    </v-card-text>

    <v-divider class="mx-4"></v-divider>

    <v-card-title>Tonight's availability</v-card-title>

    <v-card-text>
      <v-chip-group
        v-model="selection"
        active-class="deep-purple accent-4 white--text"
        column
      >
        <v-chip>5:30PM</v-chip>

        <v-chip>7:30PM</v-chip>

        <v-chip>8:00PM</v-chip>

        <v-chip>9:00PM</v-chip>
      </v-chip-group>
    </v-card-text>

    <v-card-actions>
      <v-btn
        color="deep-purple lighten-2"
        text
        @click="reserve"
      >
        Reserve
      </v-btn>
    </v-card-actions>
  </v-card>
  <v-card
    class="mx-auto"
    max-width="344"
    outlined
  >
    <v-list-item three-line>
      <v-list-item-content>
        <div class="text-overline mb-4">
          OVERLINE
        </div>
        <v-list-item-title class="text-h5 mb-1">
          Headline 5
        </v-list-item-title>
        <v-list-item-subtitle>Greyhound divisely hello coldly fonwderfully</v-list-item-subtitle>
      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="80"
        color="grey"
      ></v-list-item-avatar>
    </v-list-item>

    <v-card-actions>
      <v-btn
        outlined
        rounded
        text
      >
        Button
      </v-btn>
    </v-card-actions>
  </v-card>

  <v-card
    class="mx-auto"
    max-width="344"
  >
    <v-card-text>
      <div>Word of the Day</div>
      <p class="text-h4 text--primary">
        el·ee·mos·y·nar·y
      </p>
      <p>adjective</p>
      <div class="text--primary">
        relating to or dependent on charity; charitable.<br>
        "an eleemosynary educational institution."
      </div>
    </v-card-text>
    <v-card-actions>
      <v-btn
        text
        color="teal accent-4"
        @click="reveal = true"
      >
        Learn More
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <v-card
        v-if="reveal"
        class="transition-fast-in-fast-out v-card--reveal"
        style="height: 100%;"
      >
        <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            Origin
          </p>
          <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
        </v-card-text>
        <v-card-actions class="pt-0">
          <v-btn
            text
            color="teal accent-4"
            @click="reveal = false"
          >
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-expand-transition>
  </v-card>

  <v-row justify="space-around">
      <v-card width="400">
        <v-img
          height="200px"
          src="https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg"
        >
          <v-app-bar
            flat
            color="rgba(0, 0, 0, 0)"
          >
            <v-app-bar-nav-icon color="white"></v-app-bar-nav-icon>

            <v-toolbar-title class="text-h6 white--text pl-0">
              Messages
            </v-toolbar-title>

            <v-spacer></v-spacer>

            <v-btn
              color="white"
              icon
            >
              <v-icon>mdi-dots-vertical</v-icon>
            </v-btn>
          </v-app-bar>

          <v-card-title class="white--text mt-8">
            <v-avatar size="56">
              <img
                alt="user"
                src="https://cdn.pixabay.com/photo/2020/06/24/19/12/cabbage-5337431_1280.jpg"
              >
            </v-avatar>
            <p class="ml-3">
              John Doe
            </p>
          </v-card-title>
        </v-img>

        <v-card-text>
          <div class="font-weight-bold ml-8 mb-2">
            Today
          </div>

          <v-timeline
            align-top
            dense
          >
            <v-timeline-item
              v-for="message in messages"
              :key="message.time"
              :color="message.color"
              small
            >
              <div>
                <div class="font-weight-normal">
                  <strong>{{ message.from }}</strong> @{{ message.time }}
                </div>
                <div>{{ message.message }}</div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-card>
    </v-row>
    <v-card
      class="mx-auto"
      max-width="344"
    >
      <v-img
        src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
        height="200px"
      ></v-img>

      <v-card-title>
        Top western road trips
      </v-card-title>

      <v-card-subtitle>
        1,000 miles of wonder
      </v-card-subtitle>

      <v-card-actions>
        <v-btn
          color="orange lighten-2"
          text
        >
          Explore
        </v-btn>

        <v-spacer></v-spacer>

        <v-btn
          icon
          @click="show = !show"
        >
          <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
        </v-btn>
      </v-card-actions>

      <v-expand-transition>
        <div v-show="show">
          <v-divider></v-divider>

          <v-card-text>
            I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.
          </v-card-text>
        </div>
      </v-expand-transition>
    </v-card>
    <v-card
      class="mx-auto"
      max-width="500"
    >
      <v-system-bar
        color="indigo darken-2"
        dark
      >
        <v-spacer></v-spacer>

        <v-icon>mdi-window-minimize</v-icon>

        <v-icon>mdi-window-maximize</v-icon>

        <v-icon>mdi-close</v-icon>
      </v-system-bar>

      <v-toolbar
        color="indigo"
        dark
      >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>Discover</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
      </v-toolbar>

      <v-container fluid>
        <v-row dense>
          <v-col
            v-for="card in cards"
            :key="card.title"
            :cols="card.flex"
          >
            <v-card>
              <v-img
                :src="card.src"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
              >
                <v-card-title v-text="card.title"></v-card-title>
              </v-img>

              <v-card-actions>
                <v-spacer></v-spacer>

                <v-btn icon>
                  <v-icon>mdi-heart</v-icon>
                </v-btn>

                <v-btn icon>
                  <v-icon>mdi-bookmark</v-icon>
                </v-btn>

                <v-btn icon>
                  <v-icon>mdi-share-variant</v-icon>
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
    <v-card
      max-width="400"
      class="mx-auto"
    >
      <v-system-bar
        color="pink darken-2"
        dark
      >
        <v-spacer></v-spacer>

        <v-icon>mdi-window-minimize</v-icon>

        <v-icon>mdi-window-maximize</v-icon>

        <v-icon>mdi-close</v-icon>
      </v-system-bar>

      <v-app-bar
        dark
        color="pink"
      >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>My Music</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
      </v-app-bar>

      <v-container>
        <v-row dense>
          <v-col cols="12">
            <v-card
              color="#385F73"
              dark
            >
              <v-card-title class="text-h5">
                Unlimited music now
              </v-card-title>

              <v-card-subtitle>Listen to your favorite artists and albums whenever and wherever, online and offline.</v-card-subtitle>

              <v-card-actions>
                <v-btn text>
                  Listen Now
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col
            v-for="(item, i) in items"
            :key="i"
            cols="12"
          >
            <v-card
              :color="item.color"
              dark
            >
              <div class="d-flex flex-no-wrap justify-space-between">
                <div>
                  <v-card-title
                    class="text-h5"
                    v-text="item.title"
                  ></v-card-title>

                  <v-card-subtitle v-text="item.artist"></v-card-subtitle>

                  <v-card-actions>
                    <v-btn
                      v-if="item.artist === 'Ellie Goulding'"
                      class="ml-2 mt-3"
                      fab
                      icon
                      height="40px"
                      right
                      width="40px"
                    >
                      <v-icon>mdi-play</v-icon>
                    </v-btn>

                    <v-btn
                      v-else
                      class="ml-2 mt-5"
                      outlined
                      rounded
                      small
                    >
                      START RADIO
                    </v-btn>
                  </v-card-actions>
                </div>

                <v-avatar
                  class="ma-3"
                  size="125"
                  tile
                >
                  <v-img :src="item.src"></v-img>
                </v-avatar>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
    <v-card
      class="mx-auto"
      max-width="344"
    >
      <v-card-text>
        <div>Word of the Day</div>
        <p class="text-h4 text--primary">
          be•nev•o•lent
        </p>
        <p>adjective</p>
        <div class="text--primary">
          well meaning and kindly.<br>
          "a benevolent smile"
        </div>
      </v-card-text>
      <v-card-actions>
        <v-btn
          text
          color="deep-purple accent-4"
        >
          Learn More
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-card
      class="mx-auto"
      max-width="400"
    >
      <v-img
        class="white--text align-end"
        height="200px"
        src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
      >
        <v-card-title>Top 10 Australian beaches</v-card-title>
      </v-img>

      <v-card-subtitle class="pb-0">
        Number 10
      </v-card-subtitle>

      <v-card-text class="text--primary">
        <div>Whitehaven Beach</div>

        <div>Whitsunday Island, Whitsunday Islands</div>
      </v-card-text>

      <v-card-actions>
        <v-btn
          color="orange"
          text
        >
          Share
        </v-btn>

        <v-btn
          color="orange"
          text
        >
          Explore
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-card
      class="mx-auto"
      color="#26c6da"
      dark
      max-width="400"
    >
      <v-card-title>
        <v-icon
          large
          left
        >
          mdi-twitter
        </v-icon>
        <span class="text-h6 font-weight-light">Twitter</span>
      </v-card-title>

      <v-card-text class="text-h5 font-weight-bold">
        "Turns out semicolon-less style is easier and safer in TS because most gotcha edge cases are type invalid as well."
      </v-card-text>

      <v-card-actions>
        <v-list-item class="grow">
          <v-list-item-avatar color="grey darken-3">
            <v-img
              class="elevation-6"
              alt=""
              src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
            ></v-img>
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>Evan You</v-list-item-title>
          </v-list-item-content>

          <v-row
            align="center"
            justify="end"
          >
            <v-icon class="mr-1">
              mdi-heart
            </v-icon>
            <span class="subheading mr-2">256</span>
            <span class="mr-1">·</span>
            <v-icon class="mr-1">
              mdi-share-variant
            </v-icon>
            <span class="subheading">45</span>
          </v-row>
        </v-list-item>
      </v-card-actions>
    </v-card>
    <v-card
      class="mx-auto"
      max-width="400"
    >
      <v-list-item two-line>
        <v-list-item-content>
          <v-list-item-title class="text-h5">
            San Francisco
          </v-list-item-title>
          <v-list-item-subtitle>Mon, 12:30 PM, Mostly sunny</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-card-text>
        <v-row align="center">
          <v-col
            class="text-h2"
            cols="6"
          >
            23&deg;C
          </v-col>
          <v-col cols="6">
            <v-img
              src="https://cdn.vuetifyjs.com/images/cards/sun.png"
              alt="Sunny image"
              width="92"
            ></v-img>
          </v-col>
        </v-row>
      </v-card-text>

      <v-list-item>
        <v-list-item-icon>
          <v-icon>mdi-send</v-icon>
        </v-list-item-icon>
        <v-list-item-subtitle>23 km/h</v-list-item-subtitle>
      </v-list-item>

      <v-list-item>
        <v-list-item-icon>
          <v-icon>mdi-cloud-download</v-icon>
        </v-list-item-icon>
        <v-list-item-subtitle>48%</v-list-item-subtitle>
      </v-list-item>

      <v-slider
        v-model="time"
        :max="6"
        :tick-labels="labels"
        class="mx-4"
        ticks
      ></v-slider>

      <v-list class="transparent">
        <v-list-item
          v-for="item in forecast"
          :key="item.day"
        >
          <v-list-item-title>{{ item.day }}</v-list-item-title>

          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-subtitle class="text-right">
            {{ item.temp }}
          </v-list-item-subtitle>
        </v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-card-actions>
        <v-btn text>
          Full Report
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-carousel v-model="model">
      <v-carousel-item
        v-for="(color, i) in colors"
        :key="color"
      >
        <v-sheet
          :color="color"
          height="100%"
          tile
        >
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
            <div class="text-h2">
              Slide {{ i + 1 }}
            </div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
    <v-carousel>
      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        cover
      ></v-carousel-item>

      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/hotel.jpg"
        cover
      ></v-carousel-item>

      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
        cover
      ></v-carousel-item>
    </v-carousel>
    <v-card
      elevation="24"
      max-width="444"
      class="mx-auto"
    >
      <v-carousel
        :continuous="false"
        :show-arrows="false"
        hide-delimiter-background
        delimiter-icon="mdi-square"
        height="300"
      >
        <v-carousel-item
          v-for="(slide, i) in slides"
          :key="i"
        >
          <v-sheet
            :color="colors[i]"
            height="100%"
            tile
          >
            <div class="d-flex fill-height justify-center align-center">
              <div class="text-h2">
                {{ slide }} Slide
              </div>
            </div>
          </v-sheet>
        </v-carousel-item>
      </v-carousel>
    </v-card>
    <div class="text-center">
      <v-chip
        v-if="chip"
        class="ma-2"
        closable
        @click:close="chip = false"
      >
        Closable
      </v-chip>

      <v-btn
        v-if="!chip"
        close
        color="primary"
        dark
        @click="chip = true"
      >
        Reset Chip
      </v-btn>
    </div>
    <div class="text-center">
      <v-chip
        class="ma-2"
      >
        Default
      </v-chip>

      <v-chip
        class="ma-2"
        color="primary"
      >
        Primary
      </v-chip>

      <v-chip
        class="ma-2"
        color="secondary"
      >
        Secondary
      </v-chip>

      <v-chip
        class="ma-2"
        color="red"
        text-color="white"
      >
        Red Chip
      </v-chip>

      <v-chip
        class="ma-2"
        color="green"
        text-color="white"
      >
        Green Chip
      </v-chip>
    </div>
    <v-row
      justify="center"
      align="center"
    >
      <v-chip draggable>
        Default
      </v-chip>
    </v-row>
    <div class="text-center">
      <v-chip
        class="ma-2"
        label
      >
        Label
      </v-chip>

      <v-chip
        class="ma-2"
        color="pink"
        label
        text-color="white"
      >
        <v-icon start icon="mdi-label"></v-icon>
        Tags
      </v-chip>

      <v-chip
        class="ma-2"
        color="primary"
        label
      >
        <v-icon start icon="mdi-account-circle-outline"></v-icon>
        John Leider
      </v-chip>

      <v-chip
        class="ma-2"
        closable
        color="cyan"
        label
      >
        <v-icon start icon="mdi-twitter"></v-icon>
        New Tweets
      </v-chip>
    </div>
    <v-row
      justify="center"
      align="center"
    >
      <v-chip :ripple="false" link>
        Default
      </v-chip>
    </v-row>
    <div class="text-center">
      <v-chip
        class="ma-2"
        color="success"
        variant="outlined"
      >
        <v-icon start icon="mdi-server-plus"></v-icon>
        Server Status
      </v-chip>

      <v-chip
        class="ma-2"
        color="primary"
        variant="outlined"
      >
        User Account
        <v-icon end icon="mdi-account-outline"></v-icon>
      </v-chip>
    </div>
    <div class="text-center">
      <v-chip
        class="ma-2"
        size="x-small"
      >
        x-small chip
      </v-chip>

      <v-chip
        class="ma-2"
        size="small"
      >
        small chip
      </v-chip>

      <v-chip
        class="ma-2"
      >
        Default
      </v-chip>

      <v-chip
        class="ma-2"
        size="large"
      >
        large chip
      </v-chip>

      <v-chip
        class="ma-2"
        size="x-large"
      >
        x-large chip
      </v-chip>
    </div>
    <v-card
      class="mx-auto"
      max-width="450"
    >
      <v-img
        src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
        cover
        :aspect-ratio="16/9"
      >
      </v-img>
      <v-card-title class="flex-column align-start">
        <div class="text-h4 mb-2">
          Welcome Home...
        </div>
        <div class="text-h6 font-weight-regular text-grey">
          Monday, 12:30 PM, Mostly Sunny
        </div>
        <div class="d-flex align-center">
          <v-avatar
            size="24"
            class="me-4"
          >
            <v-img
              src="https://cdn.vuetifyjs.com/images/weather/part-cloud-48px.png"
              contain
            ></v-img>
          </v-avatar>

          <span class="text-body-2 text-grey">81° / 62°</span>
        </div>
      </v-card-title>

      <v-divider class="mx-4"></v-divider>

      <v-card-text class="d-flex justify-space-between">
        <v-chip
          prepend-icon="mdi-brightness-5"
        >
          Turn on lights
        </v-chip>
        <v-chip
          prepend-icon="mdi-alarm-check"
        >
          Set alarm
        </v-chip>
        <v-chip
          icon="mdi-blinds"
        >
          Close blinds
        </v-chip>
      </v-card-text>
    </v-card>
    <div class="text-center">
      <v-chip
        class="ma-2"
        color="indigo"
        text-color="white"
        prepend-icon="mdi-account-circle"
      >
        Mike
      </v-chip>

      <v-chip
        class="ma-2"
        color="orange"
        text-color="white"
        append-icon="mdi-star"
      >
        Premium
      </v-chip>

      <v-chip
        class="ma-2"
        color="primary"
        text-color="white"
        append-icon="mdi-cake-variant"
      >
        1 Year
      </v-chip>

      <v-chip
        class="ma-2"
        color="green"
        text-color="white"
      >
        <template v-slot:prepend>
          <v-avatar
            class="green-darken-4"
          >
            1
          </v-avatar>
        </template>
        Years
      </v-chip>

      <v-chip
        class="ma-2"
        closable
        color="teal"
        text-color="white"
        prepend-icon="mdi-checkbox-marked-circle"
        :model-value="true"
      >
        Confirmed
      </v-chip>

      <v-chip
        class="ma-2"
        closable
        color="teal"
        text-color="white"
        close-icon="mdi-delete"
        prepend-icon="mdi-checkbox-marked-circle"
        :model-value="true"
      >
        Confirmed
      </v-chip>
    </div>
    <v-card
      class="mx-auto"
      max-width="500"
    >
      <v-toolbar
        color="transparent"
        flat
      >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>Photo Info</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn
          icon="mdi-magnify"
          @click="$refs.search.focus()"
        >
        </v-btn>
      </v-toolbar>

      <v-container>
        <v-row
          align="center"
          justify="start"
        >
          <v-col
            v-for="(selection, i) in selections"
            :key="selection.text"
            cols="auto"
            class="py-1 pe-0"
          >
            <v-chip
              :disabled="loading"
              closable
              @click:close="selected.splice(i, 1)"
            >
              <v-icon
                :icon="selection.icon"
                start
              ></v-icon>

              {{ selection.text }}
            </v-chip>
          </v-col>

          <v-col
            v-if="!allSelected"
            cols="12"
          >
            <v-text-field
              ref="search"
              v-model="search"
              hide-details
              label="Search"
              single-line
            ></v-text-field>
          </v-col>
        </v-row>
      </v-container>

      <v-divider v-if="!allSelected"></v-divider>

      <v-list>
        <template v-for="item in categories">
          <v-list-item
            v-if="!selected.includes(item)"
            :key="item.text"
            :disabled="loading"
            @click="selected.push(item)"
          >
            <template v-slot:prepend>
              <v-icon
                :disabled="loading"
                :icon="item.icon"
              ></v-icon>
            </template>

            <v-list-item-title v-text="item.text"></v-list-item-title>
          </v-list-item>
        </template>
      </v-list>

      <v-divider></v-divider>

      <v-card-actions>
        <v-spacer></v-spacer>

        <v-btn
          :disabled="!selected.length"
          :loading="loading"
          color="purple"
          variant="text"
          @click="next"
        >
          Next
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-card
      class="mx-auto"
      max-width="400"
    >
      <v-row
        align="center"
        class="pa-6"
      >
        <span class="me-4">To</span>

        <v-menu
          v-model="menu"
          location="top start"
          origin="top start"
          transition="scale-transition"
        >
          <template v-slot:activator="{ props }">
            <v-chip
              pill
              v-bind="props"
              link
            >
              <v-avatar start>
                <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
              </v-avatar>

              John Leider
            </v-chip>
          </template>

          <v-card width="300">
            <v-list bg-color="black">
              <v-list-item>
                <template v-slot:prepend>
                  <v-avatar image="https://cdn.vuetifyjs.com/images/john.png"></v-avatar>
                </template>

                <v-list-item-title>John Leider</v-list-item-title>

                <v-list-item-subtitle>john@google.com</v-list-item-subtitle>

                <template v-slot:append>
                  <v-list-item-action>
                    <v-btn
                      icon
                      variant="text"
                      @click="menu = false"
                    >
                      <v-icon>mdi-close-circle</v-icon>
                    </v-btn>
                  </v-list-item-action>
                </template>
              </v-list-item>
            </v-list>

            <v-list>
              <v-list-item link prepend-icon="mdi-briefcase">
                <v-list-item-subtitle>john@gmail.com</v-list-item-subtitle>
              </v-list-item>
            </v-list>
          </v-card>
        </v-menu>
      </v-row>

      <v-divider></v-divider>

      <div class="pa-3">
        <v-text-field
          label="Subject"
          model-value="Re: Vacation Request"
          single-line
          variant="underlined"
        ></v-text-field>

        <v-textarea
          label="Message"
          single-line
          variant="underlined"
        ></v-textarea>
      </div>
    </v-card>
    <v-card
      class="mx-auto"
      max-width="450"
    >
      <v-toolbar
        color="primary"
        height="88"
        flat
      >
        <template v-slot:prepend>
          <v-btn icon="mdi-arrow-left">
          </v-btn>
        </template>

        <v-text-field
          v-model="search"
          clearable
          hide-details
          label="Search News"
          prepend-inner-icon="mdi-magnify"
          single-line
        ></v-text-field>

        <template v-slot:append>
          <v-btn icon="mdi-dots-vertical"></v-btn>
        </template>
      </v-toolbar>

      <div v-if="keywords.length > 0" class="py-3 px-4">
        <v-chip
          v-for="(keyword, i) in keywords"
          :key="i"
          class="me-2"
        >
          {{ keyword }}
        </v-chip>

      </div>

      <v-divider></v-divider>

      <v-list lines="three">
        <v-list-item
          v-for="(item, i) in searching"
          :key="i"
          link
        >
          <template v-slot:prepend>
            <v-avatar
              class="me-4 mt-2"
              rounded="0"
            >
              <v-img :src="item.image" cover></v-img>
            </v-avatar>
          </template>

          <v-list-item-title
            class="text-uppercase font-weight-regular text-caption"
            v-text="item.category"
          ></v-list-item-title>

          <div v-text="item.title"></div>
        </v-list-item>
      </v-list>
    </v-card>
    <v-combobox
      v-model="chips"
      :items="items"
      chips
      clearable
      label="Your favorite hobbies"
      multiple
      prepend-icon="mdi-filter-variant"
      variant="solo"
    >
      <template v-slot:selection="{ attrs, item, select, selected }">
        <v-chip
          v-bind="attrs"
          :model-value="selected"
          closable
          @click="select"
          @click:close="remove(item)"
        >
          <strong>{{ item }}</strong>&nbsp;
          <span>(interest)</span>
        </v-chip>
      </template>
    </v-combobox>
    <div class="d-flex justify-space-around">
      <v-color-picker
        v-model="c1"
        hide-canvas
        hide-sliders
      ></v-color-picker>

      <v-color-picker
        v-model="c2"
        hide-inputs
        show-swatches
      ></v-color-picker>
    </div>
    <div class="d-flex justify-space-around">
      <v-color-picker
        v-model="picker"
        elevation="0"
      ></v-color-picker>

      <v-color-picker
        v-model="picker"
        elevation="15"
      ></v-color-picker>
    </div>
    <v-container>
      <v-row>
        <v-col
          cols="12"
          md="4"
        >
          <v-btn class="my-4" block @click="color = null">null</v-btn>
          <v-btn class="my-4" block @click="color = '#ff00ff'">hex</v-btn>
          <v-btn class="my-4" block @click="color = '#ff00ffff'">hexa</v-btn>
          <v-btn class="my-4" block @click="color = { r: 255, g: 0, b: 255, a: 1 }">rgba</v-btn>
          <v-btn class="my-4" block @click="color = { h: 300, s: 1, l: 0.5, a: 1 }">hsla</v-btn>
          <v-btn class="my-4" block @click="color = { h: 300, s: 1, v: 1, a: 1 }">hsva</v-btn>
        </v-col>
        <v-col
          class="d-flex justify-center"
        >
          <v-color-picker v-model="color"></v-color-picker>
        </v-col>
        <v-col
          cols="12"
          md="4"
        >
          <v-sheet
            class="pa-4"
          >
            <pre>{{ color }}</pre>
          </v-sheet>
        </v-col>
      </v-row>
    </v-container>
    <div class="d-flex justify-space-around">
      <v-color-picker
        class="ma-2"
        show-swatches
        swatches-max-height="400px"
      ></v-color-picker>
      <v-color-picker
        class="ma-2"
        :swatches="swatches"
        show-swatches
      ></v-color-picker>
    </div>
    <v-card
      class="mx-auto"
      max-width="425"
    >
      <v-list lines="two">
        <v-list-subheader>Today</v-list-subheader>

        <v-list-item
          prepend-avatar="https://cdn.vuetifyjs.com/images/lists/1.jpg"
          title="Brunch this weekend?"
        >
          <template v-slot:subtitle>
            <span class="font-weight-bold">Ali Connors</span> &mdash; I'll be in your neighborhood doing errands this weekend. Do you want to hang out?
          </template>
        </v-list-item>

        <v-divider inset></v-divider>

        <v-list-item
          prepend-avatar="https://cdn.vuetifyjs.com/images/lists/2.jpg"
        >
          <template v-slot:title>
            Summer BBQ <span class="text-grey-lighten-1">4</span>
          </template>

          <template v-slot:subtitle>
            <span class="font-weight-bold">to Alex, Scott, Jennifer</span> &mdash; Wish I could come, but I'm out of town this weekend.
          </template>
        </v-list-item>

        <v-divider inset></v-divider>

        <v-list-item
          prepend-avatar="https://cdn.vuetifyjs.com/images/lists/3.jpg"
          title="Oui oui"
        >
          <template v-slot:subtitle>
            <span class="font-weight-bold">Sandra Adams</span> &mdash; Do you have Paris recommendations? Have you ever been?
          </template>
        </v-list-item>
      </v-list>
    </v-card>
    <v-toolbar color="purple">
      <template v-slot:prepend>
        <div class="text-h5">Title</div>
      </template>

      <v-divider
        class="ms-3"
        inset
        vertical
      ></v-divider>

      <v-toolbar-title>My Home</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-spacer></v-spacer>

      <v-toolbar-items>
        <v-btn variant="text">News</v-btn>

        <v-divider vertical></v-divider>

        <v-btn variant="text">Blog</v-btn>

        <v-divider vertical></v-divider>

        <v-btn variant="text">Music</v-btn>
      </v-toolbar-items>

      <v-divider vertical></v-divider>

      <v-app-bar-nav-icon class="ms-2"></v-app-bar-nav-icon>
    </v-toolbar>
    <v-card
      class="mx-auto"
      max-width="500"
    >
      <v-card-item class="bg-cyan-darken-1">
        <v-card-title>
          <span class="text-h5">Sarah Mcbeal</span>
        </v-card-title>

        <template v-slot:append>
          <v-defaults-provider
            :defaults="{
              VBtn: {
                variant: 'text',
                density: 'comfortable',
              }
            }"
          >
            <v-btn icon="mdi-chevron-left"></v-btn>

            <v-btn icon="mdi-pencil"></v-btn>

            <v-btn icon="mdi-dots-vertical"></v-btn>
          </v-defaults-provider>
        </template>
      </v-card-item>

      <v-list>
        <v-list-item
          append-icon="mdi-message-text"
          prepend-icon="mdi-phone"
          title="(650) 555-1234"
        ></v-list-item>

        <v-divider inset></v-divider>

        <v-list-item
          append-icon="mdi-message-text"
          prepend-icon="mdi-phone"
          title="(323) 555-6789"
        ></v-list-item>

        <v-divider inset></v-divider>

        <v-list-item
          prepend-icon="mdi-email"
          title="mcbeal@example.com"
        ></v-list-item>

        <v-divider inset></v-divider>

        <v-list-item
          prepend-icon="mdi-map-marker"
          title="Orlando, FL 79938"
        ></v-list-item>
      </v-list>

      <v-img
        cover
        height="200"
        src="https://picsum.photos/700?image=996"
      ></v-img>
    </v-card>
    <v-card
      class="mx-auto"
      max-width="400"
    >
      <v-toolbar
        color="orange-lighten-1"
        dark
      >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>Message Board</v-toolbar-title>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
      </v-toolbar>

      <v-list lines="two">
        <template v-for="(item, index) in items">
          <v-list-subheader
            v-if="item.header"
            :key="item.header"
            inset
          >
            {{ item.header }}
          </v-list-subheader>

          <v-divider
            v-else-if="item.divider"
            :key="index"
            inset
          ></v-divider>

          <v-list-item
            v-else
            :key="item.title"
            :prepend-avatar="item.avatar"
            ripple
          >
            <template v-slot:title>
              <div v-html="item.title"></div>
            </template>

            <template v-slot:subtitle>
              <div v-html="item.subtitle"></div>
            </template>
          </v-list-item>
        </template>
      </v-list>
    </v-card>

    <v-card>
      <v-container fluid>
        <v-row>
          <v-col cols="12">
            <v-autocomplete
              v-model="values"
              :items="items"
              label="Default"
            ></v-autocomplete>
          </v-col>

          <v-col cols="12">
            <v-autocomplete
              v-model="values"
              :items="items"
              density="comfortable"
              label="Comfortable"
            ></v-autocomplete>
          </v-col>

          <v-col cols="12">
            <v-autocomplete
              v-model="values"
              :items="items"
              density="compact"
              label="Compact"
            ></v-autocomplete>
          </v-col>
        </v-row>
      </v-container>
    </v-card>

    <v-card
      class="mx-auto"
      color="purple-lighten-1"
      max-width="500"
    >
      <v-toolbar flat color="purple">
        <v-btn icon="mdi-account"></v-btn>

        <v-toolbar-title class="font-weight-light">
          User Profile
        </v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn
          icon
          @click="isEditing = !isEditing"
        >
          <v-fade-transition leave-absolute>
            <v-icon v-if="isEditing">mdi-close</v-icon>

            <v-icon v-else>mdi-pencil</v-icon>
          </v-fade-transition>
        </v-btn>
      </v-toolbar>

      <v-card-text>
        <v-text-field
          :disabled="!isEditing"
          color="white"
          label="Name"
        ></v-text-field>

        <v-autocomplete
          :disabled="!isEditing"
          :items="states"
          :custom-filter="customFilter"
          color="white"
          item-title="name"
          item-value="abbr"
          label="State"
        ></v-autocomplete>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-actions>
        <v-spacer></v-spacer>

        <v-btn
          :disabled="!isEditing"
          @click="save"
        >
          Save
        </v-btn>
      </v-card-actions>

      <v-snackbar
        v-model="hasSaved"
        :timeout="2000"
        attach
        position="absolute"
        location="bottom left"
      >
        Your profile has been updated
      </v-snackbar>
    </v-card>
    <v-card
      :loading="isUpdating"
      color="blue-grey-darken-1"
      class="mx-auto"
      max-width="420"
    >
      <template v-slot:loader="{ isActive }">
        <v-progress-linear
          :active="isActive"
          color="green-lighten-3"
          height="4"
          indeterminate
        ></v-progress-linear>
      </template>

      <v-img
        cover
        height="200"
        src="https://cdn.vuetifyjs.com/images/cards/dark-beach.jpg"
      >
        <v-row class="pa-3">
          <v-col cols="12">
            <v-menu
              location="bottom start"
              origin="overlap"
              transition="slide-y-transition"
            >
              <template v-slot:activator="{ props }">
                <v-btn
                  v-bind="props"
                  icon="mdi-dots-vertical"
                  density="comfortable"
                  variant="tonal"
                ></v-btn>
              </template>

              <v-list :lines="false">
                <v-list-item
                  title="Update"
                  @click="isUpdating = true"
                ></v-list-item>
              </v-list>
            </v-menu>
          </v-col>

          <v-row>
            <v-col class="text-center">
              <h3 class="text-h5">{{ name }}</h3>

              <span class="text-grey-lighten-1">{{ title }}</span>
            </v-col>
          </v-row>
        </v-row>
      </v-img>

      <v-form>
        <v-container>
          <v-row dense>
            <v-col cols="12" md="6">
              <v-text-field
                v-model="name"
                :disabled="isUpdating"
                color="blue-grey-lighten-2"
                label="Name"
              ></v-text-field>
            </v-col>

            <v-col cols="12" md="6">
              <v-text-field
                v-model="title"
                :disabled="isUpdating"
                color="blue-grey-lighten-2"
                label="Title"
              ></v-text-field>
            </v-col>

            <v-col cols="12">
              <v-autocomplete
                v-model="friends"
                :disabled="isUpdating"
                :items="people"
                chips
                closable-chips
                color="blue-grey-lighten-2"
                item-title="name"
                item-value="name"
                label="Select"
                multiple
              >
                <template v-slot:chip="{ props, item }">
                  <v-chip
                    v-bind="props"
                    :prepend-avatar="item.raw.avatar"
                    :text="item.raw.name"
                  ></v-chip>
                </template>

                <template v-slot:item="{ props, item }">
                  <v-list-item
                    v-bind="props"
                    :prepend-avatar="item?.raw?.avatar"
                    :title="item?.raw?.name"
                    :subtitle="item?.raw?.group"
                  ></v-list-item>
                </template>
              </v-autocomplete>
            </v-col>
          </v-row>
        </v-container>
      </v-form>

      <v-divider></v-divider>

      <v-card-actions>
        <v-switch
          v-model="autoUpdate"
          :disabled="isUpdating"
          class="mt-0 ms-2"
          color="green-lighten-2"
          density="compact"
          hide-details
          label="Auto Update"
        ></v-switch>

        <v-spacer></v-spacer>

        <v-btn
          :disabled="autoUpdate"
          :loading="isUpdating"
          :variant="isUpdating ? 'tonal' : undefined"
          color="blue-grey-lighten-3"
          prepend-icon="mdi-update"
          @click="isUpdating = true"
        >
          Update Now
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-toolbar color="teal">
      <v-toolbar-title>State selection</v-toolbar-title>

      <v-autocomplete
        v-model="select"
        :loading="loading"
        :items="items"
        class="mx-4"
        density="comfortable"
        hide-no-data
        hide-details
        label="What state are you from?"
        style="max-width: 300px;"
      ></v-autocomplete>

      <v-btn icon="mdi-dots-vertical"></v-btn>
    </v-toolbar>
    <div>
      <v-breadcrumbs
        :items="items"
        divider="-"
      ></v-breadcrumbs>

      <v-breadcrumbs
        :items="items"
        divider="."
      ></v-breadcrumbs>

      <v-breadcrumbs :items="items">
        <template v-slot:prepend>
          <v-icon size="small" icon="mdi-vuetify"></v-icon>
        </template>
      </v-breadcrumbs>
    </div>
    <div>
      <v-breadcrumbs :items="items">
        <template v-slot:divider>
          <v-icon icon="mdi-forward"></v-icon>
        </template>
      </v-breadcrumbs>

      <v-breadcrumbs :items="items">
        <template v-slot:divider>
          <v-icon icon="mdi-chevron-right"></v-icon>
        </template>
      </v-breadcrumbs>
    </div>
    <v-breadcrumbs :items="items">
      <template v-slot:title="{ item }">
        {{ item.title.toUpperCase() }}
      </template>
    </v-breadcrumbs>
    <div>
      <v-layout style="height: 50px">
        <v-system-bar color="primary">
          <v-icon icon="mdi-wifi-strength-4" class="ms-2"></v-icon>

          <v-icon icon="mdi-signal-cellular-outline" class="ms-2"></v-icon>

          <v-icon icon="mdi-battery" class="ms-2"></v-icon>

          <span class="ms-2">08:30</span>
        </v-system-bar>
      </v-layout>

      <v-layout style="height: 50px">
        <v-system-bar color="red-lighten-2">
          <v-icon icon="mdi-wifi-strength-2" class="ms-2"></v-icon>

          <v-icon icon="mdi-signal-cellular-outline" class="ms-2"></v-icon>

          <v-icon icon="mdi-battery" class="ms-2"></v-icon>

          <span class="ms-2">18:30</span>
        </v-system-bar>
      </v-layout>

      <v-layout style="height: 50px">
        <v-system-bar color="indigo-darken-2">
          <v-icon icon="mdi-wifi-strength-3" class="ms-2"></v-icon>

          <v-icon icon="mdi-signal-cellular-outline" class="ms-2"></v-icon>

          <v-icon icon="mdi-battery" class="ms-2"></v-icon>

          <span class="ms-2">13:24</span>
        </v-system-bar>
      </v-layout>
      <v-layout style="height: 50px">
    <v-system-bar window>
      <v-icon icon="mdi-message" class="me-2"></v-icon>

      <span>10 unread messages</span>

      <v-spacer></v-spacer>

      <v-btn icon="mdi-minus" variant="text"></v-btn>

      <v-btn icon="mdi-checkbox-blank-outline" variant="text" class="ms-2"></v-btn>

      <v-btn icon="mdi-close" variant="text" class="ms-2"></v-btn>
    </v-system-bar>
  </v-layout>
  <v-row>
    <v-col
      cols="12"
      sm="6"
      class="py-2"
    >
      <p>Exclusive</p>

      <v-btn-toggle v-model="toggle_exclusive">
        <v-btn>
          <v-icon>mdi-format-align-left</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-center</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-right</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-justify</v-icon>
        </v-btn>
      </v-btn-toggle>
    </v-col>

    <v-col
      cols="12"
      sm="6"
      class="py-2"
    >
      <p>Multiple</p>

      <v-btn-toggle
        v-model="toggle_multiple"
        background-color="primary"
        dark
        multiple
      >
        <v-btn>
          <v-icon>mdi-format-bold</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-italic</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-underline</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-color-fill</v-icon>
        </v-btn>
      </v-btn-toggle>
    </v-col>

    <v-col
      cols="12"
      sm="6"
      class="py-2"
    >
      <p>No Options Selected</p>

      <v-btn-toggle v-model="toggle_none">
        <v-btn>
          <v-icon>mdi-format-align-left</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-center</v-icon>
        </v-btn>
        <v-btn>
          <v-icon>mdi-format-align-right</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-justify</v-icon>
        </v-btn>
      </v-btn-toggle>
    </v-col>

    <v-col
      cols="12"
      sm="6"
      class="py-2"
    >
      <p>Mandatory</p>

      <v-btn-toggle
        v-model="toggle_one"
        shaped
        mandatory
      >
        <v-btn>
          <v-icon>mdi-format-align-left</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-center</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-right</v-icon>
        </v-btn>

        <v-btn>
          <v-icon>mdi-format-align-justify</v-icon>
        </v-btn>
      </v-btn-toggle>
    </v-col>

    <v-col
      cols="12"
      class="py-2"
    >
      <p>Text Options</p>

      <v-btn-toggle
        v-model="text"
        rounded="0"
        color="deep-purple-accent-3"
        group
      >
        <v-btn value="left">
          Left
        </v-btn>

        <v-btn value="center">
          Center
        </v-btn>

        <v-btn value="right">
          Right
        </v-btn>

        <v-btn value="justify">
          Justify
        </v-btn>
      </v-btn-toggle>
    </v-col>

    <v-col
      cols="12"
      class="py-2"
    >
      <p>Text &amp; Icon Options</p>

      <v-btn-toggle
        v-model="icon"
        borderless
      >
        <v-btn value="left">
          <span class="hidden-sm-and-down">Left</span>

          <v-icon end>
            mdi-format-align-left
          </v-icon>
        </v-btn>

        <v-btn value="center">
          <span class="hidden-sm-and-down">Center</span>

          <v-icon end>
            mdi-format-align-center
          </v-icon>
        </v-btn>

        <v-btn value="right">
          <span class="hidden-sm-and-down">Right</span>

          <v-icon end>
            mdi-format-align-right
          </v-icon>
        </v-btn>

        <v-btn value="justify">
          <span class="hidden-sm-and-down">Justify</span>

          <v-icon end>
            mdi-format-align-justify
          </v-icon>
        </v-btn>
      </v-btn-toggle>
    </v-col>
  </v-row>

    </div>
    <v-toolbar title="Application" color="grey-lighten-3">
      <v-btn stacked>
        <v-badge
          color="error"
          dot
        >
          <v-icon icon="mdi-newspaper-variant-outline"></v-icon>
        </v-badge>

        News
      </v-btn>

      <v-btn stacked>
        <v-badge
          dot
          color="error"
        >
          <v-icon icon="mdi-post"></v-icon>
        </v-badge>

        Blog
      </v-btn>

      <v-btn
        stacked
        variant="tonal"
      >
        <v-icon icon="mdi-login"></v-icon>

        Login
      </v-btn>
    </v-toolbar>
    <v-list
      border
      class="mx-auto"
      max-width="256"
    >
      <v-list-item
        link
        prepend-icon="mdi-inbox-arrow-down"
        title="Inbox"
      >
        <template v-slot:append>
          <v-badge
            color="error"
            content="6"
            inline
          ></v-badge>
        </template>
      </v-list-item>

      <v-list-item
        link
        prepend-icon="mdi-send"
        title="Sent Mail"
      ></v-list-item>

      <v-list-item
        link
        prepend-icon="mdi-delete"
        title="Trash"
      >
        <template v-slot:append>
          <v-badge
            color="info"
            content="12"
            inline
          ></v-badge>
        </template>
      </v-list-item>

      <v-list-item
        link
        prepend-icon="mdi-alert-circle"
        title="Spam"
      ></v-list-item>
    </v-list>
    <v-toolbar color="blue-grey-darken-3">
      <v-spacer></v-spacer>

      <v-btn class="text-none" stacked>
        <v-badge dot color="success">
          <v-icon>mdi-home-outline</v-icon>
        </v-badge>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-icon>mdi-account-multiple-outline</v-icon>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-badge content="9+" color="error">
          <v-icon>mdi-store-outline</v-icon>
        </v-badge>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-badge content="2" color="error">
          <v-icon>mdi-bell-outline</v-icon>
        </v-badge>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-icon>mdi-menu</v-icon>
      </v-btn>

      <v-spacer></v-spacer>
    </v-toolbar>
    <div>
      <v-banner
        lines="one"
        icon="mdi-lock"
        color="deep-purple-accent-4"
        class="my-4"
      >
        <v-banner-text>
          Banner with one line of text.
        </v-banner-text>

        <template v-slot:actions>
          <v-btn>Action</v-btn>
        </template>
      </v-banner>

      <v-banner
        lines="two"
        icon="mdi-weather-hurricane"
        color="error"
        class="my-4"
      >
        <v-banner-text>
          Banner with two lines of text. If the text is too long to fit on two lines then an ellipsis will be used to hide the remaining content. So this next line will be hidden.
        </v-banner-text>

        <template v-slot:actions>
          <v-btn>Action</v-btn>
        </template>
      </v-banner>

      <v-banner
        lines="three"
        icon="$warning"
        color="warning"
        class="my-4"
      >
        <v-banner-text>
          Banner with three lines of text. One or two lines is preferable. Three lines should be considered the absolute maximum length on desktop in order to keep messages short and actionable.
        </v-banner-text>

        <template v-slot:actions>
          <v-btn>Action</v-btn>
        </template>
      </v-banner>
    </div>
    <v-banner
      lines="one"
      icon="mdi-wifi-strength-alert-outline"
      color="warning"
    >
      <template v-slot:text>
        No Internet connection
      </template>

      <template v-slot:actions>
        <v-btn>
          Dismiss
        </v-btn>

        <v-btn>
          Retry
        </v-btn>
      </template>
    </v-banner>
    <v-banner two-line>
      <v-avatar
        slot="icon"
        color="deep-purple accent-4"
        size="40"
      >
        <v-icon
          icon="mdi-lock"
          color="white"
        >
          mdi-lock
        </v-icon>
      </v-avatar>

      Three line text string example with two actions. One to two lines is preferable. Three lines should be considered the maximum string length on desktop in order to keep messages short and actionable.

      <template v-slot:actions>
        <v-btn
          text
          color="deep-purple accent-4"
        >
          Action
        </v-btn>
        <v-btn
          text
          color="deep-purple accent-4"
        >
          Action
        </v-btn>
      </template>
    </v-banner>
    <div>
      <v-breadcrumbs
        :items="items"
        divider="-"
      ></v-breadcrumbs>

      <v-breadcrumbs
        :items="items"
        divider="."
      ></v-breadcrumbs>
    </div>
    <div>
      <v-breadcrumbs :items="items"></v-breadcrumbs>

      <v-breadcrumbs
        :items="items"
        large
      ></v-breadcrumbs>
    </div>
    <div>
      <v-breadcrumbs :items="items">
        <template v-slot:divider>
          <v-icon>mdi-forward</v-icon>
        </template>
      </v-breadcrumbs>

      <v-breadcrumbs :items="items">
        <template v-slot:divider>
          <v-icon>mdi-chevron-right</v-icon>
        </template>
      </v-breadcrumbs>
    </div>
    <v-row justify="space-around">
      <v-icon
        large
        color="green darken-2"
      >
        mdi-domain
      </v-icon>

      <v-icon
        large
        color="blue darken-2"
      >
        mdi-message-text
      </v-icon>

      <v-icon
        large
        color="purple darken-2"
      >
        mdi-dialpad
      </v-icon>

      <v-icon
        large
        color="teal darken-2"
      >
        mdi-email
      </v-icon>

      <v-icon
        large
        color="blue-grey darken-2"
      >
        mdi-call-split
      </v-icon>

      <v-icon
        large
        color="orange darken-2"
      >
        mdi-arrow-up-bold-box-outline
      </v-icon>
    </v-row>
    <v-toolbar color="blue-grey-darken-3">
      <v-spacer></v-spacer>

      <v-btn class="text-none" stacked>
        <v-badge dot color="success">
          <v-icon>mdi-home-outline</v-icon>
        </v-badge>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-icon>mdi-account-multiple-outline</v-icon>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-badge content="9+" color="error">
          <v-icon>mdi-store-outline</v-icon>
        </v-badge>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-badge content="2" color="error">
          <v-icon>mdi-bell-outline</v-icon>
        </v-badge>
      </v-btn>

      <v-btn class="text-none" stacked>
        <v-icon>mdi-menu</v-icon>
      </v-btn>

      <v-spacer></v-spacer>
    </v-toolbar>
    <v-hover>
      <template v-slot:default="{ isHovering, props }">
        <v-card
          v-bind="props"
          :color="isHovering ? 'primary' : undefined"
          title="Hover over me"
          text="..."
        ></v-card>
      </template>
    </v-hover>
    <v-row
      align="center"
      justify="center"
    >
      <v-col cols="12">
        <v-hover
          v-slot="{ isHovering, props }"
          disabled
        >
          <v-card
            :elevation="isHovering ? 12 : 2"
            class="mx-auto"
            height="350"
            max-width="350"
            v-bind="props"
          >
            <v-card-text class="my-4 text-center text-h6">
              Hover over me!
            </v-card-text>
          </v-card>
        </v-hover>
      </v-col>
    </v-row>
    <v-responsive
      class="overflow-y-auto"
      max-height="400"
    >
      <div class="pa-6 text-center">
        Scroll down
      </div>

      <v-responsive
        height="200vh"
        class="text-center pa-2"
      >
        <v-responsive min-height="50vh"></v-responsive>
        <div class="text-center text-body-2 mb-12">
          The card will appear below:
        </div>

        <v-lazy
          v-model="isActive"
          :options="{
            threshold: .5
          }"
          min-height="200"
          transition="fade-transition"
        >
          <v-card
            class="mx-auto"
            max-width="336"
          >
            <v-card-title>Card title</v-card-title>

            <v-card-text>
              Phasellus magna. Quisque rutrum. Nunc egestas, augue at pellentesque laoreet, felis eros vehicula leo, at malesuada velit leo quis pede. Aliquam lobortis. Quisque libero metus, condimentum nec, tempor a, commodo mollis, magna.

              In turpis. In dui magna, posuere eget, vestibulum et, tempor auctor, justo. In turpis. Pellentesque dapibus hendrerit tortor. Ut varius tincidunt libero.
            </v-card-text>
          </v-card>
        </v-lazy>
      </v-responsive>
    </v-responsive>
    <v-row justify="space-around">
      <v-avatar
        color="indigo"
        size="36"
      >
        <span class="white--text text-h5">36</span>
      </v-avatar>

      <v-avatar
        color="teal"
        size="48"
      >
        <span class="white--text text-h5">48</span>
      </v-avatar>

      <v-avatar
        color="orange"
        size="62"
      >
        <span class="white--text text-h5">62</span>
      </v-avatar>
    </v-row>
    <div class="text-center">
      <v-avatar
        tile
        color="blue"
      >
        <v-icon dark>
          mdi-alarm
        </v-icon>
      </v-avatar>
    </div>
    <div class="text-center ma-2">
      <v-btn
        dark
        @click="snackbar = true"
      >
        Open Snackbar
      </v-btn>
      <v-snackbar
        v-model="snackbar"
      >
        {{ text }}

        <template v-slot:action="{ attrs }">
          <v-btn
            color="pink"
            text
            v-bind="attrs"
            @click="snackbar = false"
          >
            Close
          </v-btn>
        </template>
      </v-snackbar>
    </div>
    <div class="text-center">
      <v-btn
        dark
        color="red darken-2"
        @click="snackbar = true"
      >
        Open Snackbar
      </v-btn>

      <v-snackbar
        v-model="snackbar"
        :multi-line="multiLine"
      >
        {{ text }}

        <template v-slot:action="{ attrs }">
          <v-btn
            color="red"
            text
            v-bind="attrs"
            @click="snackbar = false"
          >
            Close
          </v-btn>
        </template>
      </v-snackbar>
    </div>
    <div class="text-center">
      <v-btn
        dark
        color="indigo"
        @click="snackbar = true"
      >
        Open Snackbar
      </v-btn>

      <v-snackbar
        v-model="snackbar"
        :vertical="vertical"
      >
        {{ text }}

        <template v-slot:action="{ attrs }">
          <v-btn
            color="indigo"
            text
            v-bind="attrs"
            @click="snackbar = false"
          >
            Close
          </v-btn>
        </template>
      </v-snackbar>
    </div>
    <v-sparkline
      :value="value"
      :gradient="gradient"
      :smooth="radius || false"
      :padding="padding"
      :line-width="width"
      :stroke-linecap="lineCap"
      :gradient-direction="gradientDirection"
      :fill="fill"
      :type="type"
      :auto-line-width="autoLineWidth"
      auto-draw
    ></v-sparkline>
    <v-card
      class="mx-auto text-center"
      color="green"
      dark
      max-width="600"
    >
      <v-card-text>
        <v-sheet color="rgba(0, 0, 0, .12)">
          <v-sparkline
            :value="value"
            color="rgba(255, 255, 255, .7)"
            height="100"
            padding="24"
            stroke-linecap="round"
            smooth
          >
            <template v-slot:label="item">
              ${{ item.value }}
            </template>
          </v-sparkline>
        </v-sheet>
      </v-card-text>

      <v-card-text>
        <div class="text-h4 font-weight-thin">
          Sales Last 24h
        </div>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-actions class="justify-center">
        <v-btn
          block
          text
        >
          Go to Report
        </v-btn>
      </v-card-actions>
    </v-card>
    <v-card
      class="mt-4 mx-auto"
      max-width="400"
    >
      <v-sheet
        class="v-sheet--offset mx-auto"
        color="cyan"
        elevation="12"
        max-width="calc(100% - 32px)"
      >
        <v-sparkline
          :labels="labels"
          :value="value"
          color="white"
          line-width="2"
          padding="16"
        ></v-sparkline>
      </v-sheet>

      <v-card-text class="pt-0">
        <div class="text-h6 font-weight-light mb-2">
          User Registrations
        </div>
        <div class="subheading font-weight-light grey--text">
          Last Campaign Performance
        </div>
        <v-divider class="my-2"></v-divider>
        <v-icon
          class="mr-2"
          small
        >
          mdi-clock
        </v-icon>
        <span class="text-caption grey--text font-weight-light">last registration 26 minutes ago</span>
      </v-card-text>
    </v-card>
    <v-card
      class="mx-auto"
      color="grey lighten-4"
      max-width="600"
    >
      <v-card-title>
        <v-icon
          :color="checking ? 'red lighten-2' : 'indigo'"
          class="mr-12"
          size="64"
          @click="takePulse"
        >
          mdi-heart-pulse
        </v-icon>
        <v-row align="start">
          <div class="text-caption grey--text text-uppercase">
            Heart rate
          </div>
          <div>
            <span
              class="text-h3 font-weight-black"
              v-text="avg || '—'"
            ></span>
            <strong v-if="avg">BPM</strong>
          </div>
        </v-row>

        <v-spacer></v-spacer>

        <v-btn
          icon
          class="align-self-start"
          size="28"
        >
          <v-icon>mdi-arrow-right-thick</v-icon>
        </v-btn>
      </v-card-title>

      <v-sheet color="transparent">
        <v-sparkline
          :key="String(avg)"
          :smooth="16"
          :gradient="['#f72047', '#ffd200', '#1feaea']"
          :line-width="3"
          :value="heartbeats"
          auto-draw
          stroke-linecap="round"
        ></v-sparkline>
      </v-sheet>
    </v-card>
    
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
