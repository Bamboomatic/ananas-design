<template>
  <div class="gallery">
  <div class="poster" v-for="image in images" :key="image.name">
    <img :alt="image.name" :src="image.url">
    <p>{{image.description}}</p>
  </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
      { name:'poster1',
        url: require('@/../public/assets/poster1.jpg'),
        description: 'MyszoJeleń'
      },
      { name:'poster2',
        url: require('@/../public/assets/poster2.jpg'),
        description: 'Wypalcowana'
      },
      { name:'poster3',
        url: require('@/../public/assets/poster3.jpg'),
        description: 'Rzuć okiem'
      },
      { name:'poster4',
        url: require('@/../public/assets/poster4.jpg'),
        description: 'Asekuracyjna'
      },
      { name:'poster5',
        url: require('@/../public/assets/poster5.jpg'),
        description: 'Myśli ulotne'
      },
      { name:'poster6',
      url: require('@/../public/assets/poster6.jpg'),
        description: 'Wichura'
      },
      { name:'poster7',
        url: require('@/../public/assets/poster7.jpg'),
        description: 'Runo'
      },
      { name:'poster8',
       url: require('@/../public/assets/poster8.jpg'),
        description: 'Splątane'
      }]
    }
  },
  methods: {
    getPic(name){
      return '../../public/assets/'+name+'.jpg'
    }
  }
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.gallery {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin: 0 auto;
  max-width: 800px;
  background: white
}

.poster {
  margin: 40px 40px 70px 40px;
  font-family: 'Praho', 'Arial Narrow', Arial, sans-serif;
  font-size: 1.6rem;
  text-shadow: 0.5px 0.5px  rgb(206, 206, 206);

}
img {
  max-width: 300px;
  box-shadow: -3px 4px 5px #383733;
  object-fit: cover;
}
</style>
