<template>
  <div class="cv-search bx--skeleton" :class="sizeClass">
    <input disabled class="bx--search-input" type="text" role="search" ref="input" />
  </div>
</template>

<script>
export default {
  name: 'CvSearchSkeleton',
  props: {
    small: { type: Boolean, default: false },
  },
  computed: {
    sizeClass() {
      return `bx--search--${this.small ? 'sm' : 'xl'}`;
    },
  },
};
</script>
