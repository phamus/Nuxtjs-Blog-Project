<template>
  <section class="posts-list">
    <PostPreview
      id="1"
      thumbnail="https://www.liberaldictionary.com/wp-content/uploads/2018/11/tech.jpg"
      postTitle="Post 1"
      postText="My First Post"
    />
    <PostPreview
      id="2"
      thumbnail="https://www.vapulus.com/en/wp-content/uploads/2019/01/tech.jpg"
      postTitle="Post 2"
      postText="My Second Post"
    />
  </section>
</template>

<script>
import PostPreview from "~/components/Posts/PostPreview";
export default {
  components: {
    PostPreview
  }
};
</script>

<style  scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
