<template>
    <span class="circle-image">
	    <img src="@/assets/woman_2.jpg" />
	</span>
</template>

<script>
//Couldn't figure out how to pass picture url using props :(
    export default{
        props:{
            pic:{
                type: String
            }
        },
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
</style>