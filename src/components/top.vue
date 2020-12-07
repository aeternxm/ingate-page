<template>
  <div class="root">
    <img src="../assets/header.png" class="top-cont">
      <div class="header">
        <img src="../assets/logo.png" class="logo"/>
        <div class="login-cont">
          <a href="https://app.ingate.com.br/login" class="login-btn">
            <img src="../assets/user.png" class="login-ico"/>
            <div class="login-name">{{login}}</div>
          </a>
        </div>
      </div>
      <div class="txt-cont">
        <div class="txt-title">{{txtTitle}}</div>
        <div class="txt-subtitle">{{txtSubtitle}}</div>
        <a href="https://app.ingate.com.br/signup" class="txt-btn">{{txtBtn}}</a>
      </div>
  </div>
</template>

<script>
export default {
  name: "top",
  props: {
    login: String,
    txtBtn: String,
    txtTitle: String,
    txtSubtitle: String,
  },
}
</script>

<style scoped>
  @media(max-width:600px) {
    .root{
      height: 100vh !important;
    }

    .top-cont{
      object-fit: cover;
      filter: brightness(0.1);
      height: 100vh !important;
    }
    .login-btn{
      padding: 2vh !important;
    }
    .login-name{
      display: none;
    }
    .txt-cont{
      justify-content: center !important;
      bottom: 20vh !important;
      width: 100vw !important;
    }
    .txt-title{
      justify-content: center !important;
      width: 100vw !important;
      margin: 0 !important;
      text-align: center !important;
    }
    .txt-subtitle{
      width: 100vw !important;
      margin: 3vh 3vw 0 3vw !important;
      text-align: center !important;
    }
    .txt-btn{
      margin: 5vh 3vw 0 3vw !important;
      width: 100vh !important;
    }
  }

  .root{
    width: 100vw;
    height: 122.5vh;
  }

  .top-cont{
    font-family: "Roboto", sans-serif;
    position: relative;
    width: 100vw;
    height: 122.5vh;
  }

  .header{
    display: flex;
    position: absolute;
    top: 2.75vh;
    width: 100vw;
    height: 10vh;
  }

  .logo{
    display: flex;
    align-self: center;
    height: 5vh;
    width: 32.34375vh;
    margin-left: 2.5vw;
  }

  .login-cont{
    display: flex;
    align-self: center;
    align-content: center;
    justify-content: flex-end;
    width: 100%;
  }

  .login-btn{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 2vh 5.25vh 2vh 5.25vh;
    margin-right: 3.5vw;
    background-color: white;
    border-radius: 5vh;
    text-decoration: none;
    transition: 0.5s;
  }

  .login-btn:hover{
    background-color: #C9C0B5;
  }

  .login-ico{
    height: 3vh;
    width: 3vh;
  }

  .login-name{
    color: black;
    margin: 0 0 0 10%;
    text-transform: uppercase;
    font-size: 2.175vh;
    font-weight: bold;
  }

  .txt-cont{
    display: flex;
    align-items: flex-start;
    justify-items: start;
    flex-flow: row wrap;
    position: absolute;
    bottom: 13vh;
    height: 54vh;
    width: 50.5vw;
  }
  
  .txt-title{
    display: flex;
    flex-flow: row wrap;
    width: 40.5vw;
    margin-left: 2.5vw;
    font-size: 2.5vh;
    text-transform: uppercase;
    text-align: start;
  }

  .txt-subtitle{
    display: flex;
    width: 40.5vw;
    margin-left: 2.5vw;
    text-align: left;
    font-family: "tiempoBolda";
    font-weight: 900;
    font-size: 5.75vh;
  }

  .txt-btn{
    display: flex;
    flex-flow: row nowrap;
    margin: 0 2.5vw 2.5vw 2.5vw;
    align-items: center;
    justify-content: center;
    padding: 3.5vh 10vh 3.5vh 10vh;
    border-radius: 1.5vh;
    background-color: white;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 2.5vh;
    font-weight: 600;
    color: black;
    transition: 0.5s;
  }

  .txt-btn:hover{
    background-color: #C9C0B5;
  }
</style>
