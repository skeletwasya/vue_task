<template>
  <div></div>
  <div className="rect">
    <div className="main-grid">
      <Description></Description>
      <Form></Form>    
    </div>
  </div>
  
     
</template>

<script>
import Form from './components/Form.vue';
import Description from './components/Description.vue';
  export default {
    components: {Form, Description},    
  }
</script>

<style>
  body{
    background: #D9D9D9;
    width: 100%;
    max-width: 100%;
    overflow-x: hidden;
  }
</style>

<style scoped>
  .rect{
    position: absolute;
    z-index: -1;
    width: 80%;
    height: 500px;
    background: white;
    
    
    top: 50%;                      
    transform: translate(0, -50%);
    border-radius: 20px;
    margin-left: 10%;
  }
  .main-grid
    {
      align-self: center;
      width: 1800px;
      height: 100%;
      display: grid;
      grid-gap: 0px;
      grid-auto-flow: column;
      padding: 50px;
      padding-left: 8%;
    }
    @media (max-width: 1800px)
    {
      .main-grid{
        width: 1500px;
      }
      
    }
    @media (max-width: 1500px)
    {
      .main-grid{
        width: 1000px;
      }
    }
    @media (max-width: 1200px)
    {
      .main-grid{
        width: 900px;
      }
    }
    @media (max-width: 1000px)
    {
      .main-grid{
        grid-auto-flow: row;
        width: 500px;
      }
      .rect{
        height: 800px;
      }
    }
    
</style>
