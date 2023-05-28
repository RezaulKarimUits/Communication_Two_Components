
<template>
<div >
<span>Receiver component {{message}}</span>
</div>
</template>

<script type="text/javascript">
import mitt from 'mitt'
const emitter = mitt()
export default {

  data() {
    return {
      message: ''

 
    };
    
    
  },

  methods: {

   
  },
  created()
  {
  },
 mounted(){
    emitter.$on('eventName', (payload) => {
      console.log("Received message", payload)
      this.message = payload.message
    });
}
};
</script>