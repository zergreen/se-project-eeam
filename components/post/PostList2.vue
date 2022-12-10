<template>
  <div style="background: blue; padding: 25px; border-radius: 15px">
    <div class="container-fluid">
      <div class="row flex-row flex-nowrap">
        <PostContent
          v-for="(my, index) in mys"
          :key="index"
          :title="my.title"
          :content="my.content"
          :score="my.score"
          :image="my.image"
          :path="my.path"
        />
      </div>
    </div>
  </div>
</template>

<script>
import PostContent from '@/components/post/PostContent'
export default {
  components: {
    PostContent,
  },
  data() {
    return {
      mys: [
        {
          title: 'kaidown',
          content: '10$',
          image:
            'https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885_960_720.jpg',
          score: '4.5',
          path: '/steak',
        },
        {
          title: 'ummm',
          content: '20$',
          image:
            'https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885_960_720.jpg',
          score: '4.5',
          path: '/steak',
        },
      ],
    }
  },
}
</script>
