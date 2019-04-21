
<template>
  <h1 class="b1" v-if="myFunction() != undefined">(UserName: {{ myFunction().split("-")[0]  }} - Lastname: {{ myFunction().split("-")[1]  }} - Id: {{ myFunction().split("-")[2]  }})</h1>
  <h1 class="b1" v-else>No User Input</h1>
</template>

<script>



export default {

  methods:{

  myFunction: function () {
  
  //console.log(window.$nuxt._route.params.id==undefined);
     
    return window.$nuxt._route.params.id;
    }
	
	},
  
  asyncData (context) {
    // called every time before loading the component
    // as the name said, it can be async
    // Also, the returned object will be merged with your data object
   
    return { name:  "World"}
  },
  fetch () {
    // The `fetch` method is used to fill the store before rendering the page
  },
 head () {
    return {
      // URL title
      title: window.location.host + this.$route.fullPath,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        // A custom description for this full path
        { hid: 'description', name: 'description', content: 'My custom description: ' +  this.$route.fullPath}
      ]
    }
  }
  // and more functionality to discover
  
}
</script>

<style>
.b1 {
  color: black;
  background-color: white;
}
</style>
