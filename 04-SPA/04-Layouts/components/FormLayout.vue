<template>
  <main class="main">
    <div class="page page_meetup-forms">
      <div class="container">
        <h2 class="page__title">{{ title }}</h2>
        <slot />
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'FormLayout',
  props: {
    title: {
      type: String,
    },
  },
};
</script>

<style scoped>
.page.page_meetup-forms {
  padding: 70px 0;
}

@media all and (max-width: 992px) {
  .page.page_meetup-forms {
    padding: 48px 0;
  }
}
</style>
