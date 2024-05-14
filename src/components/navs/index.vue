<template>
  <nav>
    <v-container class="bg pa-0">
          <div class="d-flex pa-0 justify-space-between align-center">
            <v-col cols="10" class="w-1/2">
              <!-- Menu Bar Start -->
              <ul class="d-flex justify-end ga-10">
                <li><a href="#">Home</a></li>
                <li><a href="#">About us</a></li>
                <li><a href="#">Pages</a></li>
                <li><a href="#">Our Services</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact us</a></li>
              </ul>
              <!-- Menu Bar End -->
            </v-col>
            <v-col cols="2" class="text-right ">
              <!-- Button Start -->
              <a class="btn" href="#">Have Any Questions?</a>
              <!-- Button End -->
            </v-col>
          </div>
    </v-container>
  </nav>
</template>

<script>
export default {
    name:'NavBar'
}
</script>

<style scoped>
  nav{
   position: relative;
   bottom: -55px; 
  }
  nav .bg{
    background: var(--yellow);
  }
  ul li a{
    color:var(--main);
    font-family:var(--inter);
    font-size: 20px;
    font-weight: 700;
  }
  .btn{
    display: inline-block;
    color:#ffffff;
    font-family:var(--inter);
    font-size: 20px;
    font-weight: 500;
    background: var(--main) !important;
    padding: 20px 20px;
  }
</style>