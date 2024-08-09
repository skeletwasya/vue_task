<template>
    <button @click="doSomething()" className="btn">Заказать звонок</button>
</template>

<script>
    export default{
        
    }
</script>

<style>
    .btn{
    /* Buttons/Big button */

    /* Auto layout */
    position: relative;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    

    width: 40%;
    height: 80%;
    bottom: 60%;

    /* Brand color/Green */
    background: #18A452;
    border-radius: 30px;
    border: 0;

    /* Inside auto layout */
    flex: none;
    flex-grow: 0;
    /* Button text */



    /* Desktop/Button1 */
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    line-height: 22px;
    /* identical to box height */

    /* White text/Primary */
    color: #FFFFFF;


    /* Inside auto layout */
    flex: none;
    order: 0;
    flex-grow: 0;

    

  }
  .btn:hover{
    background-color: #095f2d;
  }
  .btn:active{
    background-color: #18A452;
  }
</style>