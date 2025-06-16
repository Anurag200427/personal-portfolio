<script setup>
import AboutMe from './components/AboutMe.vue'
</script>

<template>
  <div id="app">
    <header class="header">
      <h1>My Portfolio</h1>
      <nav class="nav">
        <a href="#about" class="nav-link">About</a>
        <a href="#projects" class="nav-link">Projects</a>
        <a href="#contact" class="nav-link">Contact</a>
      </nav>
    </header>
    
    <main>
      <AboutMe />
    </main>
    
    <footer class="footer">
      <p>&copy; 2025 My Portfolio. All rights reserved.</p>
    </footer>
  </div>
</template>

<style scoped>
#app {
  max-width: 100%;
  overflow-x: hidden;
}

.header {
  background-color: #1e1e1e;
  padding: 1.5rem;
  text-align: center;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  position: sticky;
  top: 0;
  z-index: 100;
}

.nav {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 1rem;
}

.nav-link {
  color: var(--on-surface);
  text-decoration: none;
  font-weight: 500;
  padding: 0.5rem 1rem;
  border-radius: 4px;
  transition: background-color 0.2s;
}

.nav-link:hover {
  background-color: rgba(187, 134, 252, 0.1);
  color: var(--primary);
}

.footer {
  text-align: center;
  padding: 2rem 1rem;
  background-color: #1e1e1e;
  color: #888;
  margin-top: 2rem;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .nav {
    flex-direction: column;
    gap: 0.5rem;
    align-items: center;
  }
  
  .nav-link {
    width: 100%;
    text-align: center;
  }
}
</style>
