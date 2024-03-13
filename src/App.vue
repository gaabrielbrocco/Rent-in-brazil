<template>
  <v-app theme="dark">
    <v-main>
      <section id="id1">
        <v-row justify="center">
          <v-col cols="12" sm="10" md="8" lg="5" class="my-15 hover-effect">
            <v-card flat elevation="10">
              <v-card-title class="text-h4 mt-3 ml-1"
                >Casa no litoral</v-card-title
              >
              <v-card-subtitle class="text-h6 ml-1 mt-1"
                >Praia de Lages - Alagoas</v-card-subtitle
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
              <v-dialog max-width="1000" max-height="1000">
                <template v-slot:activator="{ props: activatorProps }">
                  <v-img
                    class="mt-5"
                    v-bind="activatorProps"
                    src="https://img.holidu.com/images/7ac1d603-8169-49aa-9fd4-9757f6bc51a3/l.jpg"
                  >
                  </v-img>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card>
                    <v-carousel hide-delimiters>
                      <v-carousel-item
                        v-for="(item, i) in items1"
                        :key="i"
                        :src="item.src"
                        cover
                      ></v-carousel-item>
                    </v-carousel>
                    <v-card-text  class="text-h6">
                      <v-card-title class="d-flex justify-center text-h4 mb-12"
                        >Descubra seu Refúgio Perfeito em Alagoas</v-card-title
                      >
                      <p>
                        A villa 5 é o cenário perfeito para famílias grandiosas
                        em busca de um paraíso pé na areia para chamar de seu.
                        São quatro casas idênticas, cada uma com seis suítes e
                        sua própria piscina Ou seja: é possível compartilhar
                        bons momentos ao lado de pessoas especiais, mas também
                        ter privacidade quando necessário. Recém-construída, a
                        villa 5 ainda inclui uma quadra de beach tênis e uma
                        academia.
                      </p>
                      <br />

                      <p>
                        Tudo isso, claro, embalado pela brisa e com vista para o
                        mar paradisíaco da região de São Miguel dos Milagres.
                      </p>
                    </v-card-text>

                    <v-card-actions>
                      <v-spacer></v-spacer>

                      <v-btn
                        text="Fechar"
                        color="red"
                        size="x-large"
                        @click="isActive.value = false"
                      ></v-btn>
                    </v-card-actions>
                  </v-card>
                </template>
              </v-dialog>

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
              <v-dialog max-width="1000" max-height="1000">
                <template v-slot:activator="{ props: activatorProps }">
                  <v-img
                    class="mt-5"
                    v-bind="activatorProps"
                    src="https://a0.muscache.com/im/pictures/hosting/Hosting-1027551225896727919/original/f0839dc1-8019-4d46-aee6-4a1192154c69.jpeg?im_w=720"
                  >
                  </v-img>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card>
                    <v-carousel hide-delimiters>
                      <v-carousel-item
                        v-for="(item, i) in items2"
                        :key="i"
                        :src="item.src"
                        cover
                      ></v-carousel-item>
                    </v-carousel>
                    <v-card-text  class="text-h6">
                      <v-card-title class="d-flex justify-center text-h4 mb-12"
                        >Paraíso em formato de casa</v-card-title
                      >
                      <p>
                        Venha desfrutar de momentos inesquecíveis em nossa
                        encantadora casa em Xangri-lá. Situada em uma
                        localização privilegiada, esta casa oferece todo o
                        conforto e comodidade para suas férias ou escapadas de
                        fim de semana. Com uma arquitetura moderna e espaçosa,
                        nossa casa possui ambientes cuidadosamente decorados,
                        proporcionando uma atmosfera acolhedora e relaxante.
                      </p>
                      <br />

                      <p>
                        Os amplos janelões permitem a entrada de luz natural,
                        destacando a beleza dos interiores e proporcionando
                        vistas deslumbrantes para a água.
                      </p>
                    </v-card-text>

                    <v-card-actions>
                      <v-spacer></v-spacer>

                      <v-btn
                        text="Fechar"
                        color="red"
                        size="x-large"
                        @click="isActive.value = false"
                      ></v-btn>
                    </v-card-actions>
                  </v-card>
                </template>
              </v-dialog>
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
              </div>
            </v-card>
          </v-col>
        </v-row>
        <v-row justify="center">
          <v-col cols="12" sm="10" md="8" lg="5" class="my-15 hover-effect">
            <v-card elevation="10">
              <v-card-title class="text-h4 mt-3 ml-1"
                >Casa moderna próxima do mar</v-card-title
              >
              <v-card-subtitle class="text-h6 ml-1 mt-1"
                >Floripa - SC</v-card-subtitle
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
              <v-dialog max-width="1000" max-height="1000">
                <template v-slot:activator="{ props: activatorProps }">
                  <v-img
                    class="mt-5"
                    v-bind="activatorProps"
                    src="https://img.holidu.com/images/a5413766-cd73-416f-a2a8-c3b7aeef4890/l.jpg"
                  >
                  </v-img>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card>
                    <v-carousel hide-delimiters>
                      <v-carousel-item
                        v-for="(item, i) in items3"
                        :key="i"
                        :src="item.src"
                        cover
                      ></v-carousel-item>
                    </v-carousel>
                    <v-card-text  class="text-h6">
                      <v-card-title class="d-flex justify-center text-h4 mb-12"
                        >Casa moderna à 500m do mar</v-card-title
                      >
                      <p>
                        Venha se encantar com esta casa moderna com piscina em
                        Florianópolis, onde o luxo e o conforto se encontram em
                        perfeita harmonia com a beleza natural da Ilha da Magia.
                      </p>
                      <br />

                      <p>
                        Localizada em um dos bairros mais desejados da cidade,
                        esta casa oferece uma experiência única de hospedagem
                        para quem busca sofisticação e comodidade. Ao adentrar
                        esta propriedade, você será recebido por um design
                        arrojado e contemporâneo, com espaços amplos e
                        luminosos.
                      </p>
                    </v-card-text>

                    <v-card-actions>
                      <v-spacer></v-spacer>

                      <v-btn
                        text="Fechar"
                        color="red"
                        size="x-large"
                        @click="isActive.value = false"
                      ></v-btn>
                    </v-card-actions>
                  </v-card>
                </template>
              </v-dialog>
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
              </div>
            </v-card>
          </v-col>
        </v-row>
        <v-row justify="center">
          <v-col cols="12" sm="10" md="8" lg="5" class="my-15 hover-effect">
            <v-card elevation="10">
              <v-card-title class="text-h4 mt-3 ml-1"
                >Residência com jardim</v-card-title
              >
              <v-card-subtitle class="text-h6 ml-1 mt-1"
                >Bento Gonçalves - RS</v-card-subtitle
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
              <v-dialog max-width="1000" max-height="1000">
                <template v-slot:activator="{ props: activatorProps }">
                  <v-img
                    class="mt-5"
                    v-bind="activatorProps"
                    src="https://img.holidu.com/images/f1f498a3-c72d-43ba-8d07-360404910666/l.jpg"
                  >
                  </v-img>
                </template>

                <template v-slot:default="{ isActive }">
                  <v-card>
                    <v-carousel hide-delimiters>
                      <v-carousel-item
                        v-for="(item, i) in items4"
                        :key="i"
                        :src="item.src"
                        cover
                      ></v-carousel-item>
                    </v-carousel>
                    <v-card-text  class="text-h6">
                      <v-card-title class="d-flex justify-center text-h4 mb-12"
                        >Casa com área de lazer</v-card-title
                      >
                      <p>
                        Venha conhecer esta maravilhosa casa com jardim em Bento
                        Gonçalves, um verdadeiro oásis de tranquilidade e beleza
                        no coração da região vinícola da Serra Gaúcha.
                      </p>
                      <br />

                      <p>
                        Localizada em um bairro residencial tranquilo, esta casa
                        oferece o equilíbrio perfeito entre conforto e natureza.
                        Ao adentrar o portão, você será recebido por um
                        exuberante jardim, cuidadosamente cultivado e repleto de
                        flores coloridas, árvores frutíferas e espaços para
                        relaxamento.
                      </p>
                    </v-card-text>

                    <v-card-actions>
                      <v-spacer></v-spacer>

                      <v-btn
                        text="Fechar"
                        color="red"
                        size="x-large"
                        @click="isActive.value = false"
                      ></v-btn>
                    </v-card-actions>
                  </v-card>
                </template>
              </v-dialog>
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
              </div>
            </v-card>
          </v-col>
        </v-row>
      </section>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      items1: [
        {
          src: "https://img.holidu.com/images/7ac1d603-8169-49aa-9fd4-9757f6bc51a3/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/ee600632-af01-4ca8-9559-a7c118f6b435/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/1f896ca1-10b6-4383-a445-51afc22969a2/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/93d69500-604a-442d-a1db-e6bcb3b38c24/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/53d7f180-8ae2-4579-a5a0-a5065f9b9c83/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/323ef5a1-845f-46a2-9b7f-8c057050bf1f/l.jpg",
        },
      ],
      items2: [
        {
          src: "https://a0.muscache.com/im/pictures/hosting/Hosting-1027551225896727919/original/f0839dc1-8019-4d46-aee6-4a1192154c69.jpeg?im_w=720",
        },
        {
          src: "https://a0.muscache.com/im/pictures/hosting/Hosting-1027551225896727919/original/69e6ba48-c4d1-4afa-8172-f4284e22da90.jpeg?im_w=720",
        },
        {
          src: "https://a0.muscache.com/im/pictures/hosting/Hosting-1027551225896727919/original/d07b43ba-6086-4a56-8dad-c65c384cb077.jpeg?im_w=720",
        },
        {
          src: "https://a0.muscache.com/im/pictures/hosting/Hosting-1027551225896727919/original/17ed5929-ae24-4039-aad0-dcdea9173793.jpeg?im_w=720",
        },
        {
          src: "https://a0.muscache.com/im/pictures/hosting/Hosting-1027551225896727919/original/db066ecd-cb3d-4378-8b31-908fe23c3e06.jpeg?im_w=720",
        },
      ],
      items3: [
        {
          src: "https://img.holidu.com/images/a5413766-cd73-416f-a2a8-c3b7aeef4890/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/c833a744-c1b3-45ae-ae85-1825f5207be6/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/00d5994e-88ca-4cca-a7f0-617f9cf218aa/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/052b7e6a-d8c3-4303-86af-09e21d12f5ab/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/f7d3d4aa-7624-46d8-abeb-8cc581e8b0df/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/ead5b970-8d3e-4c7e-aeb1-bd10b03977cd/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/b22376d4-0f00-4c50-90e8-61a5ed233f1a/l.jpg",
        },
      ],
      items4: [
        {
          src: "https://img.holidu.com/images/f1f498a3-c72d-43ba-8d07-360404910666/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/eb8c663c-643e-466d-937f-e5a8ae6d48ac/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/b881ee49-a6b4-4548-ad16-b83b1f4a7a65/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/96ac5384-9558-4993-b3fb-1c7885e6890a/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/80257bb9-8cc2-4462-81a5-5aa02a5cc302/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/88257f57-9986-42c3-a148-2cbce1bfb7ca/l.jpg",
        },
        {
          src: "https://img.holidu.com/images/c77a252a-1604-4037-bf3c-78079d2e70f1/l.jpg",
        },
      ],
    };
  },
};
</script>
<style scoped>
.hover-effect {
  transition: transform 0.5s ease;
}
.hover-effect:hover {
  transform: scale(1.05);
}
</style>
