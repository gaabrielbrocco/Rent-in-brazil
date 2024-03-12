<template>
  <v-app theme="dark">
    <v-main>
      <section id="id1">
        <v-row justify="center">
          <v-col cols="12" sm="10" md="8" lg="5" class="my-15 hover-effect">
            <v-card flat elevation="10">
              <v-card-title class="text-h4 mt-3 ml-1"
                >Casa de Campo</v-card-title
              >
              <v-card-subtitle class="text-h6 ml-1 mt-1"
                >Valinhos - SP</v-card-subtitle
              >
              <v-rating
                class="ml-4 mt-3"
                :model-value="4.5"
                color="amber"
                density="compact"
                size="default"
                half-increments
                readonly
              ></v-rating>
              <img
                class="mt-5"
                src="https://images.pexels.com/photos/7061663/pexels-photo-7061663.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
              />
              <div class="d-flex justify-center">
                <v-btn
                  color="blue-lighten-2"
                  icon="mdi-thumb-up"
                  size="x-large"
                  variant="text"
                ></v-btn>
                <v-btn
                  color="red-lighten-2"
                  icon="mdi-thumb-down"
                  size="x-large"
                  variant="text"
                ></v-btn>
                <v-btn
                  color="white"
                  icon="mdi-share"
                  size="x-large"
                  variant="text"
                ></v-btn>
              </div>
            </v-card>
          </v-col>
        </v-row>
        <v-row justify="center">
          <v-col cols="12" sm="10" md="8" lg="5" class="my-15 hover-effect">
            <v-card elevation="10">
              <v-card-title class="text-h4 mt-3 ml-1"
                >Residência em condomínio fechado</v-card-title
              >
              <v-card-subtitle class="text-h6 ml-1 mt-1"
                >Xangri-lá - RS</v-card-subtitle
              >
              <v-rating
                class="ml-4 mt-3"
                :model-value="3.5"
                color="amber"
                density="compact"
                size="default"
                half-increments
                readonly
              ></v-rating>
              <img
                class="mt-5"
                src="https://images.pexels.com/photos/7031577/pexels-photo-7031577.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
              />
              <div class="d-flex justify-center">
                <v-btn
                  color="blue-lighten-2"
                  icon="mdi-thumb-up"
                  size="x-large"
                  variant="text"
                ></v-btn>
                <v-btn
                  color="red-lighten-2"
                  icon="mdi-thumb-down"
                  size="x-large"
                  variant="text"
                ></v-btn>
                <v-btn
                  color="white"
                  icon="mdi-share"
                  size="x-large"
                  variant="text"
                ></v-btn>
              </div>
            </v-card>
          </v-col>
        </v-row>
        <v-row justify="center">
          <v-col cols="12" sm="10" md="8" lg="5" class="my-15 hover-effect">
            <v-card elevation="10">
              <v-card-title class="text-h4 mt-3 ml-1"
                >Casa frente mar</v-card-title
              >
              <v-card-subtitle class="text-h6 ml-1 mt-1"
                >Governador Celso Ramos - SC</v-card-subtitle
              >
              <v-rating
                class="ml-4 mt-3"
                :model-value="5"
                color="amber"
                density="compact"
                size="default"
                half-increments
                readonly
              ></v-rating>
              <img
                class="mt-5"
                src="https://images.pexels.com/photos/2476632/pexels-photo-2476632.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
              />
              <div class="d-flex justify-center">
                <v-btn
                  color="blue-lighten-2"
                  icon="mdi-thumb-up"
                  size="x-large"
                  variant="text"
                ></v-btn>
                <v-btn
                  color="red-lighten-2"
                  icon="mdi-thumb-down"
                  size="x-large"
                  variant="text"
                ></v-btn>
                <v-btn
                  color="white"
                  icon="mdi-share"
                  size="x-large"
                  variant="text"
                ></v-btn>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </section>
    </v-main>
  </v-app>
</template>

<script setup>

</script>

<style scoped>

.hover-effect {
  transition: transform 0.5s ease;
}
.hover-effect:hover {
  transform: scale(1.05);
}

</style>