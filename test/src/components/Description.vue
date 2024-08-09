<template>
    <div className="d-grid">
        <div className="description">
            <h1>Нужна консультация?</h1>
            <div>
                Оставьте номер телефона - 
                наши специалисты свяжутся с 
                вами и оперативно ответят на любой
                вопрос.
            </div>
        </div>
        
        <div className="managers">
            <Managers></Managers>
        </div>
        
    </div>   
</template>

<script>
import Managers from './Managers.vue';
    export default{
        components: {Managers},
    }
</script>

<style scoped>
    h1{
        color:#18A452;
    }
    .d-grid
    {
        display: grid;
        grid-gap: 8px;
        /* Нужна консультация? */

        font-family: Arial, Helvetica, sans-serif;          
    }
    .managers{
        width: 40%;
        height: 40%;
    }
    .description{
        width: 50%;
    }
</style>