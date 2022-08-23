<template>
<div>
Hello World <br />
{{ article }}
</div>
</template>

<script setup lang="ts">
interface Article {
  id: number
}
const article = await $fetch<Article>('https://jsonplaceholder.typicode.com/todos/1')
</script>