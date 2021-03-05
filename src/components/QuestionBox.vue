<template>
  <div>
    <b-jumbotron
    
      lead="Bootstrap v4 Components for Vue.js 2"
    >
      <template slot="lead"> 
          {{ currentQuestion.question }}
         </template>

      <hr class="my-4" />

      <p>List of answer</p>

      <b-button variant="primary" href="#">Submit</b-button>
      <b-button variant="success" @click="next" href="#">Next</b-button>
    </b-jumbotron>
  </div>
</template>    

<script>
export default {
    props: {
        currentQuestion: Object,
        next: Function
    },
    mounted: {
        
    }
}
</script>