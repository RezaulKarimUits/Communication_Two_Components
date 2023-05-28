
<template>
<div >
<span><button @click="send">Sender</button></span>
</div>
</template>

<script type="text/javascript">

export default {

  data() {
    return {
      msg:"sadi2",

 
    };
    
    
  },

  methods: {

    send() {
      console.log("Sending...")
      this.$on('eventName', {
        message: "This is a message object sent with the event"
      })
    }
   
  },
  created()
  {

    
  },
 mounted(){
    
 }
};
</script>