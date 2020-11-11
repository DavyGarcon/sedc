<template>
  <div>
    <custom-menu-item icon="dashboard" title="Vie Quotidienne"></custom-menu-item>
    <custom-menu-item icon="dashboard" title="Vie Citoyenne"></custom-menu-item>
    <custom-menu-item icon="dashboard" title="Infos Pratiques"></custom-menu-item>
    <custom-menu-item icon="dashboard" title="Culture et Loisirs"></custom-menu-item>
    <custom-menu-item icon="menu" title="Agenda"></custom-menu-item>
  </div>
</template>

<script>
import CustomMenuItem from "@/components/CustomMenuItem";

export default {
  name: "custom-menu",
  components: {
    CustomMenuItem
  }
};
</script>