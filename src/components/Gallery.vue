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
        description: 'poster 1 - milion pinionszków'
      },
      { name:'poster2',
        url: require('@/../public/assets/poster2.jpg'),
        description: 'poster 2 - milion pinionszków'
      },
      { name:'poster3',
        url: require('@/../public/assets/poster3.jpg'),
        description: 'poster 3 - milion pinionszków'
      },
      { name:'poster4',
        url: require('@/../public/assets/poster4.jpg'),
        description: 'poster 4 - milion pinionszków'
      },
      { name:'poster5',
        url: require('@/../public/assets/poster5.jpg'),
        description: 'poster 5 - milion pinionszków'
      },
      { name:'poster6',
      url: require('@/../public/assets/poster6.jpg'),
        description: 'poster 6 - milion pinionszków'
      },
      { name:'poster7',
        url: require('@/../public/assets/poster7.jpg'),
        description: 'poster 7 - milion pinionszków'
      },
      { name:'poster8',
       url: require('@/../public/assets/poster8.jpg'),
        description: 'poster 8 - milion pinionszków'
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
.poster {
  margin: 40px;
}
img {
  max-width: 260px;
  box-shadow: -3px 4px 5px #383733;
  object-fit: cover;
}
</style>
