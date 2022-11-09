<template>
    <div class="pages-hero">
      <v-container>
        <div class="d-flex align-center justify-center h-300px">
          <h2>{{title}}</h2>
        </div>
      </v-container>
      <div class="breadcrumb">
        <nuxt-link to="/">Home</nuxt-link>
        <v-icon>fas fa-arrow-right</v-icon>
        <a> {{ bredcrumb_title ? bredcrumb_title : title }} </a>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props:['title' ,'bredcrumb_title']
  }
  </script>
  
  <style lang="scss" scoped>
  .pages-hero {
    background: url("../assets/images/bg-pages-hero.svg") no-repeat;
    background-position: center;
    background-size: cover;
    position: relative;
    .h-300px {
      height: 300px;
      h2 {
        font-weight: 500;
        font-size: 36px;
        color: #fff;
      }
    }
    .breadcrumb {
      background: #fff;
      display: flex;
      align-items: center;
      justify-content: center;
      padding-right: 54px;
      padding-left: 54px;
      height: 64px;
      border-radius: 100px;
      border: 1px solid #dee2e6;
      position: absolute;
      right: 50%;
      bottom: -30px;
      transform: translateX(50%);
      font-weight: 500;
      i {
        font-size: 16px;
        margin-right: 16px;
        margin-left: 16px;
      }
      a:last-child{
        color: #6c757d;
      }
      a:first-child{
        color: #333;
      }
    }
  }
  </style>
  