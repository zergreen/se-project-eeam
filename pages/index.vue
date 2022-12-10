<template>
  <b-container fluid="md">
    <p></p>
    <h4>ร้านเทคโนอินเตอร์ ( kmitl inter food) > ไข่กระทะทรงเครื่อง</h4>
    <div class="mt-3">
      <Lineup />
    </div>
    <p></p>
    <h4>เมนูแนะนำ</h4>
    <div class="mt-3">
      <PostList />
    </div>
  </b-container>
</template>

<script>
// import PostList from '@/components/post/PostList'
import Lineup from '@/components/post/Lineup'
export default {
  components: {
    Lineup,
  },
}
</script>
