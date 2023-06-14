<template>

    <form v-on:submit.prevent="handleSubmit()">
  
      <label>Email:</label>
      <input type="email" v-model="email">
  
      <label>Message:</label>
      <textarea v-model="message"></textarea>
    
  
      <div class="submit">
          <button class="btn text-center">Submit</button>
      </div>
  
    </form>
  
  </template>
  
  <script>
  export default {
       data(){
          return{
              email: '',
              message: ''
          }
       },
       methods: {
    
          handleSubmit(){
                
                  if (!this.email !=='' && this.message !== '') {
                    alert(message + ' ' + 'is sent successfully')
                      alert('Form Submitted Successfully')
                  }
          }
       }
  }
  </script>
  
  <style>
  
  form {
      max-width: 420px;
      margin: 30px auto;
      background: white;
      text-align: left;
      padding: 0 40px 40px 40px;
      border-radius: 10px;
  }
  
  label {
      color: #aaa;
      display: inline-block;
      margin: 25px 0 15px;
      font-size: 0.6em;
      text-transform: uppercase;
      letter-spacing: 1px;
      font-weight: bold;
  }
  
 input, textarea, select {
      display: block;
      padding: 10px 6px;
      width: 100%;
      box-sizing: border-box;
      border: none;
      border-bottom: 1px solid #ddd;
      color: #555;
  }
  
 
  .submit {
    padding-top: 20px;
      text-align: center;
  }
  
  
  </style>