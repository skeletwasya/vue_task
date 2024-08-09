<template>
    <span className="m-grid">
        <div>
            <span class="circle-image">
	            <img src="@/assets/woman_1.jpg" />
	        </span>
        </div>
        <div className="middle">
            <span class="circle-image">
	            <img src="@/assets/woman_2.jpg" />
	        </span>
        </div>
        <div className="right">
            <span class="circle-image">
	            <img src="@/assets/woman_3.jpg" />
	        </span>
        </div>        
    </span>
</template>

<script>
import Photo from './Photo.vue';
    export default{
        components: {Photo},
        data(){
            return{
                pic1: "woman_1.jpg",
                pic2: "woman_2.jpg"
            }
        }
    }
</script>

<style scoped>
    .circle-image{
	  display: inline-block;
	  border-radius: 50%;
	  overflow: hidden;
	  width: 100%;
	  height: 100%;
	}
	.circle-image img{
	  width:100%;
	  height:100%;
	  object-fit: cover;
	}
    .m-grid
    {
        display: grid;
        grid-gap: 0px;
        grid-auto-flow: column;          
    }
    .middle{
        position: relative;
        left: -15%;
    }
    .right{
        position: relative;
        left: -30%;
    }
</style>