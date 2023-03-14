<template>
  <q-page class="row justify-around full-width">
    <div style="width: 50%;" class="q-pa-xl column justify-center">
      <h3 class="q-ma-none">VideoChamadas premium.</h3>
      <h3 class="q-mt-none q-mx-none">Agora gratuitas para todos.</h3>

      <span style="font-size: 20px; color: #5f6368;">Reformulamos o Google Meet, nosso serviço seguro para reuniões de negócios. Agora ele é aberto e gratuito para todos</span>
      
      <div class="row" style="margin: 70px 0px">
        <q-btn color="secondary" icon="video_call"
        class="q-mr-lg" label="Nova reunião" />
        <q-input filled v-model="text" :dense="dense" 
        label="Digite um código ou link" style="width: 300px;">
        <template v-slot:prepend>
          <q-icon name="keyboard" />
        </template>
      </q-input>
      </div>

      <q-separator class="q-mb-xl"></q-separator>

      <span style="font-size: 18px; color: #5f6368;">
       <a href="" style="color: #056B5F; text-decoration: none;">Saiba mais</a> sobre o Google Meet
      </span>
    </div>
    <div style="width: 50%;" class="row items-center justify-center">
      <q-card>
      <q-card-section class="my-card">
        <q-img src="../assets/image-right.png" width="600px"></q-img>
      </q-card-section>
    </q-card>
    </div>
     
  </q-page>
</template>

<script>

export default ({
  name: 'IndexPage',

  data() {
    return {
      text: "",
      dense: false,
    }
  }
})
</script>

<style lang="scss" scoped>
.my-card{
  .q-img{
    border-radius: 7px;
  }
}

</style>
