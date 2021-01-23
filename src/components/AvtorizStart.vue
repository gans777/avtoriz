<template>

	<div class="mt-5">
		<b-container  fluid  class="avtoriz d-flex justify-content-center" >
			<b-row>
				<b-col>
  
  <b-button variant="outline-primary" v-on:click="registration()">регистрация</b-button>
  
</b-col>
<b-col><b-button variant="outline-primary" v-on:click="Avtorization()">авторизация</b-button></b-col>
</b-row>
</b-container > 
<b-container>
<b-row v-if="reg_form">
	<b-col>
	<b-form-input  placeholder="Enter your name"></b-form-input>
	<b-form-input  placeholder="Enter your password"></b-form-input>
	<b-button variant="outline-primary" v-on:click="save_registration()">save</b-button>
	</b-col>
</b-row>
</b-container > 
</div>
</template>

<script>
	export default {
		data(){
			return {
				reg_form: false
			}
		},
		methods: {Avtorization()
      { this.reg_form=false
  },
  registration(){this.reg_form=true;
     },
    save_registration(){  	console.log("click save_registration");
    } 
  }
	}
</script>

<style>
.avtoriz {

}
</style>
