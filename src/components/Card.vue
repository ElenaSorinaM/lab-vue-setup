<template>
<Card 
      v for="post in posts"
      :title="post.title"
      :description="post.description"
      :myButton="post.button"
      @addNumber="addNumber"
      />
  
  <p> My number is {{ number }} </p>
</template>

<script>
  
	import Card from "Card.vue";
  export default {
    components: {
      Card
    },
    data(){
      return{
        posts: [
        {
        title: "Titulo 1",
        description: "Description 1",
        button: "buton 1",
        },
    
        {
        title: "Titulo 2",
        description: "Description 2",
        button: "buton 2",
        },

        {
        title: "Titulo 3",
        description: "Description 3",
        button: "buton 3",
        }
        ]
      },
    }
    
  };
</script>