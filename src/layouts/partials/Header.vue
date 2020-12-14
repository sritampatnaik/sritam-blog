<template>
  <div>
    <header class="layout-header">
      <nav class="nav">
        <g-link to="/" class="home"> 
          <svg 
            xmlns="http://www.w3.org/2000/svg" 
            fill="none" 
            width="20"
            height="20"
            viewBox="0 0 24 24" 
            stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
          </svg>
        </g-link>
        <ToggleTheme />
      </nav>
    </header>
  </div>
</template>

<script>
import ToggleTheme from "@/components/ToggleTheme";
export default {
  components: {
    ToggleTheme,
  },
};
</script>

<style>
.layout-header {
  width: 100%;
  margin: 0px auto;
  margin-top: 30px;
}
.nav {
  display: flex;
  justify-content: space-between;
}

.home {
  color: var(--text-color);
}
</style>
