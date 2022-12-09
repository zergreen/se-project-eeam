<template>
  <div style="background: #e9e9e9; padding: 25px; border-radius: 15px">
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
          title: 'ข้าวผัดกระเพราะ',
          content: 'ราคา 10 บาท',
          image:
            'https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885_960_720.jpg',
          score: '4.5',
          path: '/steak',
        },
        {
          title: 'แกงราดข้าว',
          content: 'ราคา 20 บาท',
          image:
            'https://cdn.pixabay.com/photo/2022/11/18/14/00/christmas-tree-7600201_960_720.jpg',
          score: '4.5',
          path: '/steak',
        },
        {
          title: 'ข้าวราดแกง',
          content: 'ราคา 30 บาท',
          image:
            'https://cdn.pixabay.com/photo/2022/12/05/08/54/clouds-7636282_960_720.jpg',
          score: '4.5',
          path: '/steak',
        },
      ],
    }
  },
}
</script>
