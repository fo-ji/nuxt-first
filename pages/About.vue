<template>
  <div>
    <h1>About Page</h1>
    <h2>{{ subtitle }}</h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      subtitle: 'この文章はNuxt.jsの基本的な使用法について説明しています。',
    }
  },
}
</script>
