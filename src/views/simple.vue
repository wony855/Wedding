<template>
  <div>
    <header-part></header-part>
    <contact-part></contact-part>
    <footer-part></footer-part>
  </div>
</template>

<script>
import HeaderPart from "@/components/header2.vue";
import ContactPart from "@/components/contact.vue";
import FooterPart from '@/components/footer.vue';
export default {
  components: { HeaderPart, ContactPart, FooterPart }
};
</script>

<style scoped>
</style>
