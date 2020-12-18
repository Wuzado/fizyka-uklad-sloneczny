<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title v-text="title" />
      <v-spacer />
    </v-app-bar>
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <v-footer :absolute="true" app>
      <span>
        Jan Dworakowski, &copy; {{ new Date().getFullYear() }}. Modele 3D
        pochodzą z NASA Visualization Technology Applications and Development
        (VTAD), i są udostępnione w domenie publicznej.
      </span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Wszystkie planety',
          to: '/',
        },
        {
          icon: 'mdi-weather-sunny',
          title: 'Słońce',
          to: '/slonce',
        },
        {
          icon: 'mdi-earth',
          title: 'Merkury',
          to: '/merkury',
        },
        {
          icon: 'mdi-earth',
          title: 'Wenus',
          to: '/wenus',
        },
        {
          icon: 'mdi-earth',
          title: 'Ziemia',
          to: '/ziemia',
        },
        {
          icon: 'mdi-earth',
          title: 'Mars',
          to: '/mars',
        },
        {
          icon: 'mdi-earth',
          title: 'Jowisz',
          to: '/jowisz',
        },
        {
          icon: 'mdi-earth',
          title: 'Saturn',
          to: '/saturn',
        },
        {
          icon: 'mdi-earth',
          title: 'Uran',
          to: '/uran',
        },
        {
          icon: 'mdi-earth',
          title: 'Neptun',
          to: '/neptun',
        },
        {
          icon: 'mdi-star',
          title: 'Droga Mleczna',
          to: '/droga-mleczna',
        },
      ],
      title: 'Układ słoneczny i jego planety',
    }
  },
}
</script>
