<template>
  <b-col md="3">
    <nuxt-link :to="path" style="color: inherit">
      <b-card
        :title="title"
        :img-src="image"
        img-alt="Image"
        img-top
        tag="article"
        style="max-width: 30rem"
        class="mb-2 text-center stretched-link"
      >
        <b-container class="bv-example-row">
          <b-row>
            <b-col>
              <button
                class="btn btn-primary"
                style="background: #7b0000; border-radius: 20px"
              >
                {{ score }}
              </button>
            </b-col>
            <b-col>
              <b-card-text>
                {{ content }}
              </b-card-text>
            </b-col>
          </b-row>
        </b-container>
      </b-card>
    </nuxt-link>
  </b-col>
</template>

<script>
export default {
  props: {
    imageUrl: {
      type: String,
      default: '',
    },
    path: {
      type: String,
      require: true,
    },
    title: {
      type: String,
      required: true,
    },
    score: {
      type: String,
      required: true,
    },
    content: {
      type: String,
      required: true,
    },
    image: {
      type: String,
      required: true,
    },
  },
}
</script>

<style scoped></style>
