<template>
    <transition
      enter-active-class="transition duration-300 ease-out"
      enter-from-class="translate-y-1 opacity-0"
      enter-to-class="translate-y-0 opacity-100"
      leave-active-class="transition duration-300 ease-in"
      leave-from-class="translate-y-0 opacity-100"
      leave-to-class="translate-y-1 opacity-0"
    >
      <div 
        v-show="$parent.isOpen"
        class="absolute right-0 mt-2 w-56 origin-top-right rounded-md bg-blue-100 shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none"
      >
        <slot />
      </div>
    </transition>
</template>

