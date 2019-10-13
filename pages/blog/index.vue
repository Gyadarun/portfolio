<template>
  <section id="posts">
   <PostPreview 
   v-for="post in posts"
   :key="post.id"
   :title="post.title"
   :excerpt="post.previewText"
   :thumbnailImage="post.thumbnailUrl"
   :id="post.id"
   />
  </section>
</template>

<script>
import PostPreview from '@/components/Blog/PostPreview'
export default {
  components: {
    PostPreview
  },
  data() {
    return {
      posts: [
        {
          title: 'title',
          previewText: 'preview',
          thumbnailUrl: 'https://static.mmzstatic.com/wp-content/uploads/2018/05/manquer-a-son-chat.jpg',
          id: '1'
        },
        {
          title: 'title dos',
          previewText: 'preview dos',
          thumbnailUrl: 'https://static.mmzstatic.com/wp-content/uploads/2018/05/manquer-a-son-chat.jpg',
          id: '2'
        }
      ]
    }
  }
}
</script>

<style scoped>
#posts {
  padding-top: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
@media (min-width: 35rem) {
  #posts {
    flex-direction: row;
  }
}
</style>