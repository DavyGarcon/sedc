<template>
<md-button>
  <md-icon>{{iconName}}</md-icon>
  <p>{{label}}</p>
</md-button>
</template>

<script>
export default {
  name: "custom-menu-item",
  props:{
    icon: {
      type: String,
      default: ""
    },
    title: {
      type: String,
      default: ""
    },
  },
  data: () => ({
    menuVisible: false,
    iconName: '',
    label: ''
  }),
  methods: {
    toggleMenu() {
      this.menuVisible = !this.menuVisible;
    },
    setIconName(){
      this.iconName = this.icon;
    },
    setLabel(){
      this.label = this.title;
    }    
  },
  mounted(){
    this.setIconName();
    this.setLabel();
  }
};
</script>
<style scoped>

.md-button{
  background-color: transparent !important;
  box-shadow:none;
  transition: background-color 0.8s;  
}

.md-button:hover{
  background-color: yellow !important;
  box-shadow:none;
  transition: text-decoration-line 0.5s
}

.md-button:active , .md-button:focus{
  background-color: transparent !important;  
  text-decoration-line: underline;
}
</style>