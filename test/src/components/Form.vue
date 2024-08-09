<template>
  <div className="f-grid">
      <Text :my_placeholder="txt1"></Text> 
      <Text :my_placeholder="txt2"></Text>      
      <Checkbox></Checkbox>
      <Button></Button>
      
  </div> 
</template>

<script>
import Text from './Text.vue';
import Checkbox from './Checkbox.vue';
import Button from './Button.vue';

export default{
    components: {Text, Checkbox, Button},
    data()
    {
      return{
        txt1: 'Как вас зовут?',
        txt2: '+7(999) 999-99-99',
      }
      
    }
}
</script>

<style scoped>
  *{
    margin:0;
    
  }
  .f-grid
  {
    display: grid;
    grid-gap: 8px;   
  }
  
</style>