<template>
  <svg
    :class="classes"
    xmlns="http://www.w3.org/2000/svg"
    fill="none"
    viewBox="0 0 24 24"
    stroke="currentColor"
    stroke-width="2"
  >
    <path
      stroke-linecap="round"
      stroke-linejoin="round"
      d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"
    />
    <path
      stroke-linecap="round"
      stroke-linejoin="round"
      d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
    />
  </svg>
</template>

<script>
export default {
  props: {
    colors: {
      type: String,
      default: "",
    },
    sizes: {
      type: String,
      default: "h-4 w-4",
    },
    margins: {
      type: String,
      default: "",
    },
  },

  data() {
    return {};
  },

  computed: {
    classes() {
      return this.colors + " " + this.sizes + " " + this.margins;
    },
  },
};
</script>
