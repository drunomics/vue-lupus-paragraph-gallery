<template>
  <div class="paragraph paragraph--gallery">
    <slot name="field_media"/>
    <slot/>
  </div>
</template>
<script>
  export default {
    name: 'PgGallery',
  };
</script>
