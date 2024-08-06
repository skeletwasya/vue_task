<template>
  <div>
    <input type="text" v-model="name" placeholder="Как вас зовут">
  </div> 
  <div>
    <input type="text" v-model="phoneNumber" placeholder="+7(999) 999-99-99">
  </div>
  <div>
    <input type="checkbox" id="checkbox" v-model="checkboxClicked">
    <label for="checkbox">Даю согласие на обработку моих персональных данных, с условиями политики ознакомлен</label>
  </div>
  <div>
    <button @click="doSomething()">Заказать звонок</button>
  </div>
  <p>{{ error }}</p>
</template>

<script>
  export default {
    data()
    {
      return{
        error: '',
        name: '',
        phoneNumber: '',
        checkboxClicked: false
      }
    },
    methods:
    {
      doSomething()
      {
        if(this.name != '' && this.phoneNumber != '' && this.checkboxClicked)
        {
          console.log("something")
          this.name = ''
          this.phoneNumber = ''
          this.error = ''
        }
        else
        {
          this.error = 'Неверно введены данные!'
          return
        }      
      }
    }
  }
</script>

<style scoped>
  
</style>
