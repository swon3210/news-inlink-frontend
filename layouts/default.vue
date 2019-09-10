<template>
  <v-app>
    <v-navigation-drawer
      v-model="drawerRight"
      app
      clipped
      right
    >
      <v-list dense>
        <v-list-item @click.stop="right = !right">
          <v-list-item-action>
            <v-icon>mdi-exit-to-app</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>신문사 바꾸기</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-list>
        <v-list-item-group
          v-model="model2"
          v-for="(item, i) in items3"
          :key="i"
        >
            <v-divider
              :key="`divider-${i}`"
            ></v-divider>

            <v-list-item
              :key="`item-${i}`"
              :value="item"
              active-class="deep-purple--text text--accent-4"
            >
              <v-list-item-content>
                <v-list-item-title v-text="item"></v-list-item-title>
              </v-list-item-content>
            </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      app
      clipped-right
      color="blue-grey"
      dark
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>네이버 뉴스</v-toolbar-title>
      <div class="flex-grow-1"></div>
      <v-app-bar-nav-icon @click.stop="drawerRight = !drawerRight"></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-list dense>
        <v-list-item 
          v-for="item in items"
          :key="item.id"
          :to="item.to"
        >
          <v-list-item-action>
            <v-icon>{{item.icon}}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>{{item.title}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-navigation-drawer
      v-model="left"
      fixed
      temporary
    ></v-navigation-drawer>

    <v-content>
      <nuxt />
    </v-content>

    <v-navigation-drawer
      v-model="right"
      fixed
      right
      temporary
    >
      <v-list>
        <v-list-item-group v-model="model">
          <v-list-item
            v-for="(item, i) in items2"
            :key="i"
          >
            <v-list-item-icon>
              <v-icon v-text="item.icon"></v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title v-text="item.text"></v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <!-- <v-footer
      app
      color="blue-grey"
      class="white--text"
    >
      <span>Vuetify</span>
      <div class="flex-grow-1"></div>
      <span>&copy; 2019</span>
    </v-footer> -->
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          icon: 'mdi-apps',
          title: '뉴스',
          to: '/'
        },
        {
          icon: 'mdi-apps',
          title: '소개',
          to: '/intro'
        },
      ],
      model: 1,
      items2: [
        {
          icon: 'mdi-inbox',
          text: 'A',
        },
        {
          icon: 'mdi-star',
          text: 'B',
        },
        {
          icon: 'mdi-send',
          text: 'C',
        },
        {
          icon: 'mdi-email-open',
          text: 'D',
        },
      ],
      items3: [
        '최근 기사 1',
        '최근 기사 2',
        '최근 기사 3',
        '최근 기사 4',
        '최근 기사 5',
      ],
      model2: ['Carrots'],
      drawer: true,
      drawerRight: true,
      right: false,
      left: false,
    }
  }
}
</script>
