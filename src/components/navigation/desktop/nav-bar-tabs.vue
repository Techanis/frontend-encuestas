<template>
  <div class="nav-bar__tabs">
    <NavBarTab path="/public" label="Noticias" />
    <template v-if="isAuthenticated">
      <NavBarTab path="/profile" label="Perfil" />
      <NavBarTab path="/protected" label="Concursos" />
      <NavBarTab path="/admin" label="Admin" />
    </template>
  </div>
</template>

<script setup>
import NavBarTab from "@/components/navigation/desktop/nav-bar-tab.vue";
import { useAuth0 } from "@auth0/auth0-vue";

const { isAuthenticated } = useAuth0();
</script>