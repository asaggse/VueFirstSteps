<template>
	<section>
    
  	<p v-if="likes > 0">
    	this video has {{ likes }} 👍🏻
  	</p>
    
    <p v-else>
    	nobody likes it 😭
  	</p>
    
    <button v-on:click="likeAndSubscribe()">
      Like & Subscribe 👍🏻
    </button>
    
  </section>
</template>

<script>
export default {
  
  data() {
    return {
      likes: 0,
    }
  },
  
  methods: {
    likeAndSubscribe() {
      this.likes++;
      alert('Thanks! Have some cake 🍰')
    }
  }
  
}
</script>