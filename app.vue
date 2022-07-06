<template>
  <div>
    {{ cookie }}
  </div>
</template>

<script lang="ts" setup>
  const { cookie } = useRequestHeaders(['cookie'])
  console.log(cookie) // prints "undefined" for curl calls without cookie header
</script>
