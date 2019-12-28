<template>
  <div>
    <h2>Group Foo</h2>
    <div class="sub-nav">
      <ul>
        <li><NuxtLink to="/group-foo/foo-a">foo A</NuxtLink></li>
        <li><NuxtLink to="/group-foo/foo-b">foo B</NuxtLink></li>
      </ul>
    </div>
    <hr />
    <nuxt-child />
  </div>
</template>

<script>
export default {
  transition: {
    name: 'slide-right'
  }
}
</script>
