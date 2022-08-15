<template>
  <main>
    <div class="container">
      <h1>seja muito bem vindo</h1>
      <img
        :src="img"
        alt="imagem bolada do dragon ball"
      />
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugiat ab, sed
        consectetur, eaque nesciunt sequi nihil cumque voluptas quis velit quia
        asperiores, culpa tenetur! Quae, ea? Dignissimos, quos consequuntur
        eligendi voluptate expedita ea? Suscipit optio quidem odio dolor,
        eligendi commodi necessitatibus autem similique maiores dolorum aliquam
        aut quis, nisi doloribus.
      </p>
    </div>
  </main>
</template>

<script>
export default {
  name: "HomeView",
  components: {},
  data(){
    return{
      imgList: [
        'http://pm1.narvii.com/7828/849557d07a9390fc03b546f24fca611a7ac51640r1-736-670v2_uhq.jpg',
        'https://sm.ign.com/t/ign_latam/screenshot/default/gohan-goku-vegeta_1bhd.620.png',
        'https://i.uai.com.br/uMklJyrxS3sB4Xg0I9EjDhSG3Fg=/1200x675/smart/imgsapp2.uai.com.br/app/noticia_133890394703/2022/06/08/287174/goku-e-vegeta-sao-personagens-de-dragon-ball_1_104617.jpg',
       ],
       img: '',
       count: 0
    }
  },
  mounted() {
    this.img = this.imgList[this.count]
    setInterval(()=>{
      if(this.count > 2){
        this.count = 0
      }else{
        this.img = this.imgList[this.count]
        this.count++
      }
    }, 3000)
},
};
</script>

<style scoped>
main{
  width: 100%
}
  .container{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 20px;
  }
  h1{
    text-transform: uppercase;
  }
  img{
    width: 100%;
    max-width: 700px;
    height: 700px;
    background-size: contain;
    background-position: center;
  }p{
    width: 100%;
    max-width: 800px;
    text-align: center;
  }
</style>
