<template>
    <div class="pages-hero" :style="{ 'background-image': 'url(' + post_image + ')' }">
        <v-container>
            <div class="d-flex align-center justify-center h-300px">
                <h2>{{ title }}</h2>
            </div>
        </v-container>
        <div class="breadcrumb">
            <nuxt-link to="/blog">
                Blog
            </nuxt-link>
            <v-icon>fas fa-arrow-right</v-icon>
            <nuxt-link to="/">
                {{ category }}
            </nuxt-link>
        </div>
        <div class="overlay" />
    </div>
</template>

<script>
export default { props: ['title', 'category', 'post_image'] }
</script>

<style lang="scss" scoped>
.pages-hero {
  background-position: center;
  margin-bottom: 66px;
  background-size: cover;
  position: relative;
  .overlay {
    background: #000;
    position: absolute;
    opacity: 0.46;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
  }
  .h-300px {
    z-index: 10000;
    height: 330px;
    h2 {
      font-weight: 500;
      z-index: 10000;
      font-size: 36px;
      color: #fff;
    }
  }
  .breadcrumb {
    z-index: 1000;
    background: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    padding-right: 45px;
    padding-left: 45px;
    height: 60px;
    border-radius: 100px;
    border: 1px solid #dee2e6;
    position: absolute;
    right: 50%;
    bottom: -30px;
    transform: translateX(50%);
    i {
      font-size: 16px;
      margin-right: 12px;
      margin-left: 12px;
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
