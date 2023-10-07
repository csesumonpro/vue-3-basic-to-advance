<template>
<div class="container">
    Slots Component
  <header>
    <slot name="header" :user="user" headerContent="HeaderContent Data" ></slot>
  </header>
  <main>
    <slot userName="sumon"></slot>
  </main>
  <footer>
    <slot name="footer"></slot>
  </footer>
</div>
</template>

<script setup>

const user = {
    name: 'sumon',
    email: 'sumon@gmail.com'
}
</script>