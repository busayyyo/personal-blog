<template>
  <Layout :show-logo="false">
    <!-- Author intro -->
    <Author :show-title="true" />
    
    <!--<div v-for="edge in $page.posts.edges">
      <PostTags :post="edge.node" />
    </div>-->

    <!-- List posts -->
    <div class="posts">
      <PostCard v-for="edge in $page.posts.edges" :key="edge.node.id" :post="edge.node"/>
    </div>

  </Layout>
</template>

<page-query>
query {
  posts: allPost(filter: { published: { eq: true }}) {
    edges {
      node {
        id
        title
        date (format: "D. MMMM YYYY")
        timeToRead
        description
        ...on Post {
        id
        title
        path
        }
        path
        tags {
          id
          title
          path
        }
      }
    }
  }
}
</page-query>

<script>
import Author from '~/components/Author.vue'
import PostCard from '~/components/PostCard.vue'
import PostTags from '~/components/PostTags.vue'

export default {
  components: {
    Author,
    PostCard,
    PostTags
  },
  metaInfo: {
    title: 'Home'
  }
}
</script>
