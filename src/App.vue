<template>
  <v-app>
    <app-navbar />
    <v-main>
      <v-container>
        <v-row>
          <v-col cols="12" md="6">
            <h1 class="mt-16 ml-16">Delicious Food Is <br/>Waiting For You </h1>
            <p class="mt-16 ml-16">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.<br/>
              Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, <br/>
              when an unknown printer took a galley of type and scrambled it to make a type specimen book. 
            </p>
            <v-btn class="mt-8 ml-16 rounded-pill" color="#9B7150">
              Foot Menu
            </v-btn>
            <v-btn class="mt-8 ml-16 rounded-pill" color="#9B7150">
              Book a Table
            </v-btn> 
          </v-col>
          <v-col cols="12" md="6">
            <v-img src="/1.jpg" :width="500" aspect-ratio="16/9" cover></v-img>
          </v-col>
          <v-col cols="12" md="12">
            <h2 class="text-center">Top list</h2>
            <h2 class="text-center">Our mainstay menu</h2>
          </v-col>
          <v-col cols="12" sm="4" class="d-flex justify-center">
            <v-card color="transparent" max-width="200" flat>
              <v-img src="/1.jpg" height="70" class="image"></v-img>
              <v-card class="mt-n10 rounded-xl" max-width="300" color="#CDAC8B">
                <v-card-item class="text-center">
                  <v-cart-title class="mt-10">Noodles three</v-cart-title>
                  <v-cart-subtitle class="mt-10">
                    <span class="me-1">White plate with <br/> dried shrimps</span>
                  </v-cart-subtitle>
                  <v-cart-title>12$</v-cart-title>
                </v-card-item>
                <v-card-text>
                  <v-row align="center" class="mx-0">
                    <v-icon color="yellow" icon="mdi mdi-star"></v-icon>
                    <div class="ms-4">
                      <h6>8.1</h6>
                    </div>
                    <v-spacer></v-spacer>
                    <div class="text-grey ms-4">
                      <v-icon color="brown">mdi mdi-plus-circle</v-icon>
                    </div>
                  </v-row>
                </v-card-text>
              </v-card>
            </v-card>
          </v-col>
          <v-col cols="12" sm="4" class="d-flex justify-center">
            <v-card color="transparent" max-width="200" flat>
              <v-img src="/1.jpg" height="70" class="image"></v-img>
              <v-card class="mt-n10 rounded-xl" max-width="300" color="#CDAC8B">
                <v-card-item class="text-center">
                  <v-cart-title class="mt-10">Noodles three</v-cart-title>
                  <v-cart-subtitle class="mt-10">
                    <span class="me-1">White plate with <br/> dried shrimps</span>
                  </v-cart-subtitle>
                  <v-cart-title>12$</v-cart-title>
                </v-card-item>
                <v-card-text>
                  <v-row align="center" class="mx-0">
                    <v-icon color="yellow" icon="mdi mdi-star"></v-icon>
                    <div class="ms-4">
                      <h6>8.1</h6>
                    </div>
                    <v-spacer></v-spacer>
                    <div class="text-grey ms-4">
                      <v-icon color="brown">mdi mdi-plus-circle</v-icon>
                    </div>
                  </v-row>
                </v-card-text>
              </v-card>
            </v-card>
          </v-col>
          <v-col cols="12" sm="4" class="d-flex justify-center">
            <v-card color="transparent" max-width="200" flat>
              <v-img src="/1.jpg" height="70" class="image"></v-img>
              <v-card class="mt-n10 rounded-xl" max-width="300" color="#CDAC8B">
                <v-card-item class="text-center">
                  <v-cart-title class="mt-10">Noodles three</v-cart-title>
                  <v-cart-subtitle class="mt-10">
                    <span class="me-1">White plate with <br/> dried shrimps</span>
                  </v-cart-subtitle>
                  <v-cart-title>12$</v-cart-title>
                </v-card-item>
                <v-card-text>
                  <v-row align="center" class="mx-0">
                    <v-icon color="yellow" icon="mdi mdi-star"></v-icon>
                    <div class="ms-4">
                      <h6>8.1</h6>
                    </div>
                    <v-spacer></v-spacer>
                    <div class="text-grey ms-4">
                      <v-icon color="brown">mdi mdi-plus-circle</v-icon>
                    </div>
                  </v-row>
                </v-card-text>
              </v-card>
            </v-card>
          </v-col>
          <v-col cols="12" md="6">
            <v-img src="/1.jpg" :width="500" aspect-ratio="16/9" cover></v-img>
          </v-col>
          <v-col cols="">
            <h1 style="margin-top: 100px;">This is title<br/> and subtitle</h1>
            <p class="mt-6">
              Lorem Ipsum is simply dummy text of the printing and typesetting industry.<br/>
              Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, <br/>
              when an unknown printer took a galley of type and scrambled it to make a type specimen book. 
            </p>
          </v-col>
          <v-col cols="12" md="12">
            <h1 class="text-center">Our services</h1>
          </v-col>
          <v-col cols="12" md="12">
            <div class="d-flex justify-space-evenly mt-4" color="transparent">
              <v-chip class="ma-2" color="black" variant="outlined" v-for="(food, i) in foods" :key="i">
                <v-icon :icon="food.icon" start></v-icon> {{ food.title }}
              </v-chip>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script setup>
  const foods = [
    {title: "Outline booking", icon: "mdi mdi-cellphone-sound"},
    {title: "Catering service", icon: "mdi mdi-food-outline"},
    {title: "Membership", icon: "mdi mdi-account-group"},
    {title: "Delivery service", icon: "mdi mdi-truck-delivery-outline"},
  ];
</script>
<style scoped>
  .image {
    z-index: 9999 !important;
  }
</style>