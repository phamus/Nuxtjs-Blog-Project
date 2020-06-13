<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest News</h1>
    </section>
    <section class="featured-posts">
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
  </div>
</template>

<script>
import PostPreview from "~/components/Posts/PostPreview";
export default {
  components: {
    PostPreview
  }
};
</script>


<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url("~assets/images/main-page-background.jpg");
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px #7a7575;
  box-sizing: border-box;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
