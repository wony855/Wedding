<template>
  <div>
    <header-part></header-part>
    <calendar-part></calendar-part>
    <map-part></map-part>
    <account-part></account-part>
    <contact-part></contact-part>
    <footer-part></footer-part>
  </div>
</template>

<script>
import HeaderPart from "@/components/header.vue";
import CalendarPart from '@/components/calendar.vue';
import MapPart from "@/components/map.vue";
import AccountPart from "@/components/account.vue";
import ContactPart from "@/components/contact.vue";
import FooterPart from '@/components/footer.vue';
export default {
  components: { HeaderPart, CalendarPart, MapPart, AccountPart, ContactPart, FooterPart }
};
</script>

<style scoped>
</style>
