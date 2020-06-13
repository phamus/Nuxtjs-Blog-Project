<template>
  <div class="admin-new-post-page">
    <section class="new-post-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "~/components/Admin/AdminPostForm";
export default {
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: "Phamus",
        title: "Skype",
        thumbnailLink:
          "https://www.liberaldictionary.com/wp-content/uploads/2018/11/tech.jpg",
        content: "Nice post"
      }
    };
  }
};
</script>
