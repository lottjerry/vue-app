<template>
  <div>
    <MenuView v-slot:default="slotProps" class="relative inline-block text-left">
    <MenuButton  class="inline-flex w-full justify-center rounded-md bg-blue-900 px-4 py-2 text-sm font-bold text-white hover:bg-opacity-70 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75">Options</MenuButton>
      <MenuItems v-if="slotProps.isOpen">
        <MenuItem class="cursor-pointer text-blue-900 font-bold group flex w-full items-center rounded-md px-2 py-2 text-sm hover:bg-blue-900 hover:text-white">Account Settings</MenuItem>
        <MenuItem class="cursor-pointer text-blue-900 font-bold group flex w-full items-center rounded-md px-2 py-2 text-sm hover:bg-blue-900 hover:text-white">Support</MenuItem>
        <MenuItem class="cursor-pointer text-blue-900 font-bold group flex w-full items-center rounded-md px-2 py-2 text-sm hover:bg-blue-900 hover:text-white">License</MenuItem>
        <MenuItem class="cursor-pointer text-blue-900 font-bold group flex w-full items-center rounded-md px-2 py-2 text-sm hover:bg-blue-900 hover:text-white">Sign Out</MenuItem>
      </MenuItems>
    </MenuView>
  </div>
</template>

<script>
  import MenuView from './MenuView.vue'
  import MenuButton from './MenuButton.vue'
  import MenuItems from './MenuItems.vue'
  import MenuItem from './MenuItem.vue'

  export default {
    components: {
      MenuView,
      MenuButton,
      MenuItems,
      MenuItem,
    }
  }
</script>
