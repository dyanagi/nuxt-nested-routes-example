<template>
  <div class="nav">
    <h1>The Navigation</h1>
    <ul>
      <li><NuxtLink to="/">Home</NuxtLink></li>
      <li><NuxtLink to="/group-foo">Group Foo</NuxtLink></li>
      <li><NuxtLink to="/group-bar">Group Bar</NuxtLink></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'TheNavigation'
}
</script>
