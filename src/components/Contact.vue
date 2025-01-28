<script>
export default {
  name: 'HsFormComponent',
  mounted() {
    // Dynamically load the external script
    const script = document.createElement('script')
    script.src = 'https://js.hsforms.net/forms/embed/48878841.js'
    script.defer = true
    document.head.appendChild(script)
  },
}
</script>

<template>
  <a name="contact-us">
    <div class="isolate bg-white px-6 py-6 lg:px-48">
      <div
        class="hs-form-frame"
        data-region="na1"
        data-form-id="4a9d1812-ab9d-45ef-98d0-d9ba97bde30c"
        data-portal-id="48878841"
      ></div>
    </div>
  </a>
</template>
