<template>
  <div>
    <NavbarView> 
      <NavbarButton> </NavbarButton>

      <NavbarItems> 
        <NavbarItem> </NavbarItem>
        <NavbarItem> </NavbarItem>
        <NavbarItem> </NavbarItem>
      </NavbarItems>

      <MenuComponent />
    </NavbarView>
  </div>
</template>

<script>
import NavbarView from './NavbarView.vue'
import NavbarButton from './NavbarButton.vue'
import NavbarItems from './NavbarItems.vue'
import NavbarItem from './NavbarItem.vue'
import MenuComponent from '../Menu/MenuComponent.vue'

  export default {
    components: {
      NavbarView,
      NavbarButton,
      NavbarItems,
      NavbarItem,
      MenuComponent,
    },

    data () {
      return {
        links: [
          {name: "Home", link: "#"},
          {name: "About", link: "#"},
          {name: "Contact", link: "#"},
        ]
      }
    }
  }
</script>

