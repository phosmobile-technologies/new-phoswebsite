<template>
      <Layout>
         <BlogList></BlogList>
      </Layout>
</template>

<page-query>
query blogData {
  blogdata: allBlogData {
    edges{
      node{
        id,
        title,
        path
      }
    }
  }
}
</page-query>

<script>
import BlogList from '../components/BlogList'
export default {
   metaInfo: {
    title: 'Blog'
  },
  components: {
     BlogList
  }
}
</script>

<style>

</style>