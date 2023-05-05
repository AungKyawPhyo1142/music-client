<template>
  <TopNavigation></TopNavigation>
  <div id="accountView" class="max-w-4xl mx-auto">
    <router-view></router-view>
  </div>
  <FooterSection></FooterSection>
</template>

<style lang="scss">
#accountView{
  min-height: 70vh;
}
</style>

<script setup>
  import TopNavigation from '@/components/structure/TopNavigation.vue';
  import FooterSection from '@/components/structure/FooterSection.vue';
</script>