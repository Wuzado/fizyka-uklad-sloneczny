<template>
  <v-row justify="center" align="center">
    <v-col v-for="planet in planets" :key="planet.name" cols="12" sm="8" md="6">
      <v-card>
        <v-card-title> {{ planet.name }} </v-card-title>
        <iframe
          :src="planet.model"
          width="100%"
          height="450px"
          frameborder="0"
        />
        <!--<v-card-text> {{ planet.desc }} </v-card-text>-->
        <v-card-actions>
          <v-btn nuxt :to="planet.link">
            <v-icon> mdi-information </v-icon>
            Więcej informacji
          </v-btn>
          <v-btn :href="planet.wiki">
            <v-icon> mdi-wikipedia </v-icon>
            Wikipedia
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      planets: [
        {
          name: 'Słońce',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2352',
          desc: 'info',
          link: '/slonce',
          wiki: 'https://pl.wikipedia.org/wiki/S%C5%82o%C5%84ce',
        },
        {
          name: 'Merkury',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2369',
          desc: 'info',
          link: '/merkury',
          wiki: 'https://pl.wikipedia.org/wiki/Merkury',
        },
        {
          name: 'Wenus',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2343',
          desc: 'info',
          link: '/wenus',
          wiki: 'https://pl.wikipedia.org/wiki/Wenus',
        },
        {
          name: 'Ziemia',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2393',
          desc: 'info',
          link: '/ziemia',
          wiki: 'https://pl.wikipedia.org/wiki/Ziemia',
        },
        {
          name: 'Mars',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2372',
          desc: 'info',
          link: '/mars',
          wiki: 'https://pl.wikipedia.org/wiki/Mars',
        },
        {
          name: 'Jowisz',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2375',
          desc: 'info',
          link: '/jowisz',
          wiki: 'https://pl.wikipedia.org/wiki/Jowisz',
        },
        {
          name: 'Saturn',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2355',
          desc: 'info',
          link: '/saturn',
          wiki: 'https://pl.wikipedia.org/wiki/Saturn',
        },
        {
          name: 'Uran',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2344',
          desc: 'info',
          link: '/uran',
          wiki: 'https://pl.wikipedia.org/wiki/Uran',
        },
        {
          name: 'Neptun',
          model: 'https://solarsystem.nasa.gov/gltf_embed/2364',
          desc: 'info',
          link: '/neptun',
          wiki: 'https://pl.wikipedia.org/wiki/Neptun',
        },
      ],
    }
  },
}
</script>
