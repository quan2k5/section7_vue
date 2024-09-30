<script setup>
</script>
<template>
<div>
    <header>
        <slot  name="header"></slot>
    </header>
    <body>
          <slot  name="body"></slot>
    </body>
    <footer>
        <slot  name="footer"></slot>
    </footer>
</div>
</template>
<style scoped></style>