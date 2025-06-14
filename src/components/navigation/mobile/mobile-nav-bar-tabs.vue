<template>
  <div class="mobile-nav-bar__tabs">
    <MobileNavBarTab path="/public" label="Noticias" />
    <template v-if="isAuthenticated">
      <MobileNavBarTab path="/profile" label="Perfil" />
      <MobileNavBarTab path="/protected" label="Concursos" />
      <MobileNavBarTab path="/admin" label="Admin" />
    </template>
  </div>
</template>

<script setup>
import MobileNavBarTab from "@/components/navigation/mobile/mobile-nav-bar-tab.vue";
import { useAuth0 } from "@auth0/auth0-vue";

const { isAuthenticated } = useAuth0();
</script>

<style scoped></style>