<template>
  <div>
    <h2>Group Bar</h2>
    <div class="sub-nav">
      <ul>
        <li><NuxtLink to="/group-bar/bar-a">bar A</NuxtLink></li>
        <li><NuxtLink to="/group-bar/bar-b">bar B</NuxtLink></li>
      </ul>
    </div>
    <hr />
    <nuxt-child />
  </div>
</template>

<script>
export default {
  transition: {
    name: 'swipe-right'
  }
}
</script>
