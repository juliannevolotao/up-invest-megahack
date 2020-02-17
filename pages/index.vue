<template>
  <main class="container">

    <section class="left">
      <div class="left-logo"></div>
      <div class="left-texto"> 
        <h1> Aprenda, 
          <br> Invista & 
          <br> Transforme!
        </h1>
      </div>

      <div class="left-buttons">
        <div class="button">
          <p> Acessar conta </p>
        </div>
        <div class="button">
          <p> Criar conta </p>
        </div>
      </div>

    </section>

    <section class="right">
    </section>
    
  </main>
</template>

<script>

export default {
  
}
</script>

<style scoped>

  *{
    font-family: 'Roboto', sans-serif;
  }

  .container {
    width: 100%;
    max-width: 1024px;
    height: 620px;
    margin: 60px auto;
    background-color: #F2F2F2;
    border-radius: 5px;
    display: flex;
  }

  .left{
    position: relative;
    width: 50%;
    height: 100%;
    padding: 50px 60px;
    display: flex;
    flex-direction: column;
  }

  .left-logo{
    width: 140px;
    height: 140px;
    background-image: url("../static/logoColorido.png");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;

  }

  .left-texto {
    padding-left: 30px;
    margin-top: 30px;
    font-size: 24px;
    line-height: 45px;
    color: #01C676;
  }

  .left-buttons {
    margin: 60px 0 0 30px;
    height: 60px;
    width: 320px;
    position: relative;
    display: flex;
    justify-content: space-between;
  }

  .button{
    position: relative;
    border: #01C676 3px solid;
    border-radius: 5px;
    height: 100%;
    width: 150px;
    display: flex;
    text-align: center;
    padding: 10px;
    cursor: pointer;
    transition: all .4s;
  }

  .button:hover {
    transform: scale(1.08);
  }

  .button p {
    width: 124px;
    line-height: 36px;
    color: #4A4A4A;
    font-weight: bold;
  }

  .right {
    position: relative;
    width: 50%;
    background-image: url("../static/fundoMulher.png");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 100%;
  }
</style>>


