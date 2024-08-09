<template>
    <input type="text" v-model="name" className="txt" :placeholder="my_placeholder" >
</template>

<script>
    export default{
        props: {
            my_placeholder: {
                type: String
            }
        }
    }
</script>

<style scoped>
    .txt{
    /* Placeholder/Default */

    /* Auto layout */
    border: 0;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    padding: 0px;

    width: 40%;
    height: 40%;


    /* Inside auto layout */
    flex: none;
    flex-grow: 1;

    /* Text Fields/1 value */

    /* Auto layout */
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 12px 16px;
    gap: 16px;

    /* Background/Secondary */
    background: #F6F6F6;
    border-radius: 8px;

    /* Inside auto layout */
    flex: none;
    order: 0;
    flex-grow: 0;
  }
  .txt:focus{
    outline: none;
    border: 2px solid #18A452;
  }
  @media (max-width: 1000px)
    {
      .txt{
        width: 40%;
      }
    }
</style>