<template>
  <section id="subscribe_sec">
    <v-container>
        <v-row  align="center">
            <v-col cols="8">
                <h4>Subscribe Our Newsletter</h4>
                <p><span>stay in touch with us to get latest news.</span> maximus mattis est facilisi. In sed pretium Proin pretium id urna sit amet tincidunt.</p>
            </v-col>
            <v-col cols="4">
                <div class="sbsrbe_inp">
                    <form action="#" method="post">
                        <input type="text" placeholder="">
                        <button>Subscribe</button>
                    </form>
                </div>
            </v-col>
        </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
    name:'SubscribeComp'
}
</script>

<style scoped>
    #subscribe_sec{
        background: var(--yellow);
        padding: 40px 0;
    }
    h4{
        font-family: var(--mulish);
        font-size: 45px;
        font-weight: 900;
        color: var(--main);
    }
    p{
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--main);
        max-width: 585px;
    }
    p span{
        font-weight: 700;
    }
    .sbsrbe_inp input{
        width: 400px;
        background: transparent;
        border: 2px solid #ffffff;
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 400;
        color: var(--main);
        padding: 10px 20px;
    }
    .sbsrbe_inp input:focus{
        outline: none;
    }
    .sbsrbe_inp button{
        background: #ffffff;
        border: 1px solid #ffffff;
        font-family: var(--inter);
        font-size: 18px;
        font-weight: 700;
        color: var(--main);
        padding: 11px 20px;
    }
</style>