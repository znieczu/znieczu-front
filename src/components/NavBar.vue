<template>
    <div class="navbar">
      <img id="logo" src="../assets/znieczu-logo.png" width="80" height="80">

      <div class="navbar-buttons">
            <router-link to="/" tag="button">Home</router-link>
            <router-link to="/about-us" tag="button">About Us</router-link>
            <img src="../assets/znieczu-logo.png" width="80" height="80">
            <button>Our Products</button>
          <button>Contacts</button>

        </div>

    </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style>
  #logo {
    display: none;
  }
    .navbar {
        border-bottom: solid 1px #EBEAEA;
        padding: 30px;
        font-weight: bold;
    }

    button {
        background-color: white;
        border: None;
        margin: 10px;
        font-size: 15px;
        font-weight: bold;
    }
    .button-znieczu {
        background-color: rgba(0,0,0,0.7);
        color: #fff;
        padding: 30px;
    }
    .navbar-buttons {
        display: flex;
        justify-content: space-around;
    }

    @media screen and (max-width: 600px) {
      .navbar {
        border-bottom: solid 1px #EBEAEA;
        padding: unset;
        font-weight: bold;
      }
      .navbar-buttons {
        display: flex;
        flex-direction: column;
      }
      .navbar-buttons > img {
        display: none;
      }
      .button-znieczu {
        background-color: rgba(0,0,0,0.7);
        color: #fff;
        padding: 30px;
      }
      #logo {
        display: unset;
      }
    }
</style>
