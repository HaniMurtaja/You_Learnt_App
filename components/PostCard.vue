<template>
    <div class="blog-post" :class="grid ? 'flex-column' : 'flex-row'">
        <v-img :width="grid ? '100%' : '30%'" :height="grid ? '220px' : '255px'" src="http://akwade.net/youlearnt/assets/img/post-blog-2.png" />
        <div class="content">
            <h5 class="primary--text">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            </h5>
            <span class="textdark--text">
                November 29, 2019
            </span>
            <p class="textmuted--text">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur distinctio ea excepturi facere fugiat ipsum laboriosam laudantium molestias necessitatibus nesciunt non
            </p>
            <nuxt-link class="primary--text" to="#">
                Continue Reading
            </nuxt-link>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        grid: {
            type: Boolean,
            default: false,
        },
    },
}
</script>

<style lang="scss" scoped>
  .blog-post {
    border: 1px solid #ccc;
    border-radius: 6px;
    display: flex;
    margin-bottom: 16px;
    overflow: hidden;
    align-items: center;
    @media(max-width: 776px) {display: block;height: auto}
    .content {
      padding: 20px;
      h5 {
        font-size: 20px;
        line-height: 1.2;
        font-weight: 500;
        padding: 0;
        margin: 0;
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        -webkit-line-clamp: 2; /* number of lines to show */
        line-clamp: 2;
        -webkit-box-orient: vertical;
      }
      span {
        display: block;
        font-size: 13px;
        margin: 12px 0;
      }
      p {
        padding: 0;
        margin: 0;
        font-size: 14px;
        line-height: 20px;
        color: #ABABAB !important;
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        -webkit-line-clamp: 3; /* number of lines to show */
        line-clamp: 3;
        height: 60px;
        -webkit-box-orient: vertical;
      }
      a {
        font-size: 14px;
        font-weight: 500;
        margin-top: 16px;
        display: block;
      }
    }

  }
</style>
