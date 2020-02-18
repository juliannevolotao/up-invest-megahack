<template lang="pug">
  main.container

    section.left

      div(v-if="!logarConta && !criarConta").inicial-content
        div.left-logo
          img(src="../static/logoCortado.png")
        div.left-texto
          p UpInvest
          h1 
            | Aprenda, 
            br 
            | Invista &
            br
            | Transforme!

        div.left-buttons

          div( @click="logarConta = true").button
            a Acessar conta

          div( @click="criarConta = true").button
            a Cadastrar



      div(v-if="logarConta").login-content

        span( @click="logarConta = false" ).arrow-back 
          <svg xmlns="http://www.w3.org/2000/svg" width="10.079" height="16.608" viewBox="0 0 10.079 16.608"><defs><style>.a{fill:#01c676;}</style></defs><path class="a" d="M27.76,45.321l7.391-7.391a.913.913,0,0,1,1.291,0l.862.862a.913.913,0,0,1,0,1.289l-5.858,5.885,5.858,5.885a.912.912,0,0,1,0,1.289L36.441,54a.913.913,0,0,1-1.291,0L27.76,46.612A.913.913,0,0,1,27.76,45.321Z" transform="translate(-27.492 -37.662)"/></svg>
          span Voltar

        div.left-logo.logosmall
          img(src="../static/logoCortado.png")

        div.login-texto
          h2 Olá
          span Seja bem vindo novamente!

        input(type="text" placeholder="Seu CPF").input
        input(type="password" placeholder="Sua senha").input

        span.esqueceu-senha Esqueceu a senha?

        div.btnLogar
          nuxt-link( to="/dashboard" style="text-decoration: none")
            div( @click="").button
                a Entrar

        span.semconta Ainda não tenho conta: 
          span( @click="criarConta = true, logarConta = false") cadastre-se


      div(v-if="criarConta").cadastro-content

        span( @click="logarConta = false, criarConta = false" ).arrow-back 
          <svg xmlns="http://www.w3.org/2000/svg" width="10.079" height="16.608" viewBox="0 0 10.079 16.608"><defs><style>.a{fill:#01c676;}</style></defs><path class="a" d="M27.76,45.321l7.391-7.391a.913.913,0,0,1,1.291,0l.862.862a.913.913,0,0,1,0,1.289l-5.858,5.885,5.858,5.885a.912.912,0,0,1,0,1.289L36.441,54a.913.913,0,0,1-1.291,0L27.76,46.612A.913.913,0,0,1,27.76,45.321Z" transform="translate(-27.492 -37.662)"/></svg>
          span Voltar

        div.left-logo.logosmall
          img(src="../static/logoCortado.png")

        div.cadastro-texto
          h2 Olá
          span Eu sou o MoneyBot e vi que você 
            br
            | está querendo ter uma conta nova.
            br 
            br 
            | Infelizmente nós não estamos criando contas no momento,
            | mas em 
            font breve 
            | nós poderemos conversar um pouco mais, 
            br
            | 
            font até logo!



    section.right
    
  </main>
</template>

<script>
export default {
  head() {
        return {
            title: 'UpInvest'
        }
        
  },
  data() {
    return {
      logarConta: false,
      criarConta: false,
    }
  }
}
</script>

<style lang="sass" scoped>

  @keyframes fade
    0% 
        transform: translateX(10px)
        opacity: 0
    100% 
        transform: translateX(0px)
        opacity: 1
  

  .container
    animation: fade .8s
    overflow-x: hidden
    width: 100%
    justify-content: space-between
    height: 100%
    background-color: #F2F2F2
    border-radius: 5px
    display: flex
    box-sizing: border-box

    .left
      position: relative
      padding: 60px
      width: 35%
      justify-content: center
      display: flex
      flex-direction: column
      box-sizing: border-box
      margin-left: auto

      input 
        width: 270px
        height: 50px
        border-radius: 4px
        border: 3px solid #01C676
        background-color: transparent
        outline: none
        box-sizing: border-box
        padding: 4px 12px
        font-size: 1em
        margin: 0 0 20px 0

      .logosmall 
          width: 80px !important
          height: 80px !important
          margin: 30px 0

      .left-logo
        width: 128px
        height: 138px
        
        img 
          width: 100%


      .inicial-content
        display: flex
        flex-direction: column
        justify-content: center
        width: 100%

        

        .left-texto
          //padding-left: 30px
          margin-top: 60px
          font-size: 24px
          line-height: 45px
          color: #01C676

          h1 
            text-align: left

        .left-buttons
          margin: 50px 0 0 0
          height: 60px
          width: 320px
          position: relative
          display: flex
          justify-content: flex-start

          
      
      .login-content
        display: flex
        flex-direction: column
        justify-content: center
        width: 100%

        .login-texto 
          //padding-left: 30px
          margin-bottom: 30px

          h2
            color: #01C676
            font-size: 24px
            margin-top: 30px

          span 
            color: #4A4A4A
            font-size: 18px

        .esqueceu-senha
          //padding-left: 30px
          font-size: 12px
          color: #01c576
          margin-top: -10px

        .btnLogar
          margin: 80px 0 0 60px
          width: 140px

        .semconta
          font-size: 12px
          margin-left: 25px
          margin-top: 10px
          color: #A4A4A4

          span
            color: #01c576
            cursor: pointer

        
      .cadastro-content
        display: flex
        flex-direction: column
        justify-content: center
        width: 100%

        .cadastro-texto 
          //padding-left: 30px
          margin-bottom: 30px

          h2
            color: #01C676
            font-size: 24px
            margin-top: 30px

          span 
            color: #4A4A4A
            font-size: 18px

            font 
              color: #01C676
          
    

    .right
      position: relative
      width: 55%
      background-image: url("../static/fundooval.jpg")
      background-size: cover
      background-repeat: no-repeat
      height: 100%




    .arrow-back 
      //padding-left: 30px
      font-size: 1em
      color: #01C676
      display: flex
      margin-bottom: 20px
      width: fit-content
      cursor: pointer
      transition: all .4s

      span 
        margin-left: 5px

      &:hover 
        transform: scale(1.07)

    .button
      position: relative
      border: #01C676 3px solid
      border-radius: 5px
      height: 50px
      width: auto
      display: flex
      text-align: center
      padding: 10px 18px
      cursor: pointer
      transition: all .4s
      justify-content: center
      text-decoration: none

      &:first-of-type
        margin-right: 20px

      &:hover 
        transform: scale(1.08)
    
      a
        line-height: 24px
        color: #4A4A4A
        font-weight: bold
        text-decoration: none
      
    
</style>


