<script setup>
import { ref } from 'vue'
import Home from './Home.vue'
import Staking from './Staking.vue'
import Links from './Links.vue'
import About from './About.vue'
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
import { MailOutlined, AppstoreOutlined, SettingOutlined } from '@ant-design/icons-vue';


const myCarousel = ref(null);

const toHomeClick = () => {
  myCarousel.value.slideTo(0)
}
const toStakingClick = () => {
  myCarousel.value.slideTo(1)
}
const toLinksClick = () => {
  myCarousel.value.slideTo(2)
}
const toAboutClick = () => {
  myCarousel.value.slideTo(3)
}
const pages = [Home, Staking, Links, About]

</script>

<template>
  <a-layout>
    <a-layout-header>
    <div id="menu">
      <a-menu v-model:selectedKeys="current" mode="horizontal">
        <a-menu-item @click="toHomeClick" key="home">
          Home
        </a-menu-item>
        <a-menu-item @click="toStakingClick" key="staking">
          Staking
        </a-menu-item>
        <a-menu-item @click="toLinksClick" key="link">
          Links
        </a-menu-item>
        <a-menu-item @click="toAboutClick" key="about">
          About
        </a-menu-item>
      </a-menu>
    </div>
    </a-layout-header>
    <a-layout-content >
      <carousel ref="myCarousel" :mouseDrag="false" :touchDrag="false" :transition="800">
        <slide v-for="slideName in pages" :key="slideName">
            <component v-bind:is="slideName" ></component>
        </slide>
      </carousel>


    </a-layout-content>
  </a-layout>
</template>

<style>
.ant-layout {
  width: 100%;
  height: 100vh;
}


#menu ul {
  background-color: transparent;
  position: absolute;
  z-index: 1;
  color: #fff;
  font-size: 1.3rem;
  width: 100%;
  font-weight: 400;
  font-family: 'Courier New',
    Courier,
    monospace;
}

#menu ul li:hover{
  color: yellow;
}

#menu .ant-menu-horizontal:not(.ant-menu-dark)>.ant-menu-item-selected {
  color: yellow;
}


#menu .ant-menu-horizontal:not(.ant-menu-dark)>.ant-menu-item-selected::after {
  border-bottom: 2px solid yellow;
}


.ant-layout .ant-layout-header {
  height: 15vh;
  padding: 2vh 2vw !important;
  color: rgba(0, 0, 0, 0.85);
  line-height: 64px;
  background: transparent;
}

.ant-layout .ant-layout-header .ant-menu-horizontal {
  border: none;
}

.ant-layout .ant-layout-content {
height: 100vh;
margin-top: -20vh;
overflow: hidden;
}
</style>
