<template>
    <label className="container"> 
        Даю 
        <a href="https://www.google.com/">согласие</a> 
        на обработку моих персональных данных, с условиями 
        <a href="https://www.google.com/">политики</a> ознакомлен
        <input type="checkbox">
        <span class="checkmark"></span>
    </label>
</template>

<script>
    export default{
        
    }
</script>

<style scoped>
    a{
    text-decoration: none;
    color:#18A452;
    }
    a:active{
        color: #000;
    }
    a:hover {
    text-decoration: underline;
   }
    a:visited{
        color:#18A452;
    }
    label{
    /* Text line */
    /* Desktop/Text2 */
    font-family: Arial, Helvetica, sans-serif;
    font-size: 14px;

    /* Black text/Primary */
    color: #212121;


    /* Inside auto layout */

    }
     /* Customize the label (the container) */
    .container {
    display: block;
    position: relative;
    padding-left: 35px;
    margin-bottom: 12px;
    cursor: pointer;
    font-size: 22px;
    
    width: 45%;
    }

    /* Hide the browser's default checkbox */
    .container input {
    position: absolute;
    opacity: 0;
    cursor: pointer;
    height: 0;
    width: 0;
    }

    /* Create a custom checkbox */
    .checkmark {
    position: absolute;
    top: 0;
    left: 0;
    height: 25px;
    width: 25px;
    background-color: #eee;
    }

    /* On mouse-over, add a grey background color */
    .container:hover input ~ .checkmark {
    background-color: #ccc;
    }

    /* When the checkbox is checked, add a blue background */
    .container input:checked ~ .checkmark {
    background-color: #18A452;
    }

    /* Create the checkmark/indicator (hidden when not checked) */
    .checkmark:after {
    content: "";
    position: absolute;
    display: none;
    }

    /* Show the checkmark when checked */
    .container input:checked ~ .checkmark:after {
    display: block;
    }

    /* Style the checkmark/indicator */
    .container .checkmark:after {
    left: 9px;
    top: 5px;
    width: 5px;
    height: 10px;
    border: solid white;
    border-width: 0 3px 3px 0;
    -webkit-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    transform: rotate(45deg);
    }
    @media (max-width: 1500px)
    {
      .container{
        font-size: 12px;
        
      }
    }

</style>