<template>
    <div class="home">
        <div class="container">
            <div class="carrols-image">
                <carousel-3d :controlsVisible="true" :autoplay="true" :autoplayTimeout=5000>
                    <slide :index="0" :height="700">
                        <img src="../assets/dubai.jpg" :height="300">
                    </slide>
                    <slide :index="1" :height="700">
                        <img src="../assets/london.jpg" :height="300">
                    </slide>
                    <slide :index="2" :height="700">
                        <img src="../assets/newyork.jpg" :height="300">>
                    </slide>
                </carousel-3d>
            </div>
            <div class="info">
                <br><br>
                <div class="description">
                    <p>
                        Description znieczu project Description znieczu project Description znieczu project Description znieczu project
                        Description znieczu project Description znieczu project Description znieczu project Description znieczu project
                        Description znieczu project Description znieczu project Description znieczu project Description znieczu project
                        Description znieczu project Description znieczu project Description znieczu project Description znieczu project
                    </p>
                </div>
                <div class="logInUp">
                    <button class="signUpButton">Sign Up</button>
                    <h4>Or</h4>
                    <button class="loginButton">Login</button>
                </div>
            </div>
        </div>
        <br>
        <br>
        <Skills/>

    </div>
</template>

<script>
import Skills from './HomeComponents/Skills'
import { Carousel3d, Slide } from 'vue-carousel-3d'

export default {
  name: 'Home',
  components: {
    Skills,
    Carousel3d,
    Slide
  }
}
</script>

<style>
    .container {
        width:100%;
        height: 70vh;
        background-color: white;
        display: flex;
    }
    .carrols-image, .info {
        width: 50%;
        height: 50vh;
        margin: 20px;
    }
    .info {
        background-color: white;
        font-size: 13px;
        text-align: center;
        margin: 20px;
        flex-direction:column;
    }
    .logInUp {
        align-items: flex-end;
    }

    .loginButton, .signUpButton {
        background-color: rgba(0,0,0,0.7);
        color: white;
        padding: 20px 45px 20px 45px;
    }
    .signUpButton {
        background-color: #3a5180;
    }
</style>
