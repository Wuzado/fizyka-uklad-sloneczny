<template>
  <v-row justify="center">
    <v-col cols="12" sm="8" md="6">
      <v-card>
        <v-card-title> Ziemia </v-card-title>
        <iframe
          src="https://solarsystem.nasa.gov/gltf_embed/2393"
          width="100%"
          height="450px"
          frameborder="0"
        />
      </v-card>
      <v-card>
        <v-img
          lazy-src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/97/The_Earth_seen_from_Apollo_17.jpg/480px-The_Earth_seen_from_Apollo_17.jpg"
          src="https://upload.wikimedia.org/wikipedia/commons/9/97/The_Earth_seen_from_Apollo_17.jpg"
          alt="The Blue Marble"
        />
        <v-card-subtitle>
          The Blue Marble - zdjęcie Ziemi wykonane 7 grudnia 1972 o 5:39 EST
          (10:39 UTC) przez załogę Apollo 17.
        </v-card-subtitle>
      </v-card>
    </v-col>
    <v-col cols="12" sm="8" md="6">
      <v-card>
        <v-card-title> Opis </v-card-title>
        <v-card-text>
          <b>Ziemia</b> jest trzecią planetą (planeta skalista) od Słońca w
          Układzie Słonecznym, i jedyną, na której powierzchni odnotowano życie.
        </v-card-text>
        <v-card-text> <b>Aphelium:</b> 152 100 000 km </v-card-text>
        <v-card-text> <b>Peryhelium:</b> 147 095 000 km </v-card-text>
        <v-card-text>
          <b>Masa Ziemi:</b> 5,97237×10<sup>24</sup> kg
        </v-card-text>
        <v-card-text>
          <b>Grawitacja na powierzchni:</b> 9,807 m/s<sup>2</sup>
        </v-card-text>
        <v-card-text>
          <b>Okres orbity wokół Słońca:</b> 365.256363004 dnia
        </v-card-text>
        <v-card-text>
          <b>Okres obrotu wokół własnej osi (dzień):</b> 23 godziny 56 minuty
          4,100 sekundy
        </v-card-text>
        <v-card-text>
          <b>Liczba naturalnych satelitów:</b> jeden (Księżyc)
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>
