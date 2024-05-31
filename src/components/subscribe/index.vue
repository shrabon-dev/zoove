<template>
  <section id="subscribe_sec">
    <v-container>
        <v-row  align="center" align-md="end" align-lg="center">
            <v-col cols="12" md="8" lg="8">
                <h4>Subscribe Our Newsletter</h4>
                <p><span>stay in touch with us to get latest news.</span> maximus mattis est facilisi. In sed pretium Proin pretium id urna sit amet tincidunt.</p>
            </v-col>
            <v-col cols="12" md="4" lg='4'>
                <div class="sbsrbe_inp text-md-end">
                    <form action="#" method="post">
                        <input type="text" placeholder="">
                        <button class="mt-1 mt-lg-0">Subscribe</button>
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
        max-width: 400px;
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
    @media (min-width:300px) and (max-width:600px){
        #subscribe_sec{
            padding: 20px 0;
        }
        h4{
            font-size: 32px;
            line-height: 1.3;
        }
        p{
            font-size: 14px;
        }
    }
</style>