<template>
    <div class="navbar">
        <div class="navbar-buttons">
            <button>Home</button>
            <button>Company</button>
            <img src="../assets/znieczu-logo.png" width="80" height="80">
            <button>Our Products</button>
            <button>About Us</button>
        </div>
    </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style>
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
</style>
