<template>
  <section class="admin-wrapper">
    <section>
      <header class="form-header">
        <h3>Add New Book</h3>
      </header>
      <form class="form-wrapper" @submit.prevent="handleSubmit">
        <div class="form-image">
          <img class="image-preview" src="{image}" alt="" />
          <input type="file" accept="image/jpg" @change="handleImageUpload" />
        </div>
        <div class="form-fields">
          <div class="title-form">
            <p><label htmlFor="title">Title</label></p>
            <p>
              <input
                type="title"
                placeholder="Type the title"
                v-model="form.title"
              />
            </p>
          </div>
          <div class="description-form">
            <p><label htmlFor="description">Description</label></p>
            <p>
              <textarea
                type="text"
                rows="8"
                placeholder="Type the description of the book"
                v-model="form.BookDescription"
              />
            </p>
          </div>
          <div class="author-form">
            <p><label htmlFor="author">Author</label></p>
            <p>
              <input
                type="text"
                placeholder="Type the author's
                name"
                v-model="form.Bookauthor"
              />
            </p>
          </div>
          <div class="price-form">
            <p>
              <label htmlFor="price">Price ($)</label>
              <input
                type="text"
                placeholder="What is the Price of the book (USD)"
                v-model="form.BookPrice"
              />
            </p>
          </div>
          <div class="featured-form">
            <p>
              <label>Featured?</label>
              <input type="checkbox" v-model="form.checked" />
            </p>
          </div>
          <div class="submit-form">
            <button class="btn" type="submit">Submit</button>
          </div>
        </div>
      </form>
    </section>
  </section>
</template>

<script>
export default {
  data: () => ({
    form: {
      title: "",
      BookDescription: "",
      Bookauthor: "",
      BookPrice: "",
      checked: false,
    },
  }),
  methods: {
    async handleSubmit() {
      try {
      } catch (error) {
        console.log({ error });
      }
    },
    async handleImageUpload() {
      try {
      } catch (error) {}
    },
  },
};
</script>

<style>
</style>
