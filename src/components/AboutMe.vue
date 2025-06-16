<template>
  <section id="about" class="about-section">
    <div class="about-container">
      <h2 class="section-title">About Me</h2>
      <div class="about-content">
        <div class="about-image">
          <img src="../assets/me.jpg" alt="Profile Picture" class="profile-pic">
        </div>
        <div class="about-text">
          <p>Hello! I'm a passionate developer with expertise in web development and a keen eye for design. I love creating responsive and user-friendly applications that make a difference.</p>
          <div class="skills">
            <h3>Skills</h3>
            <div class="skills-grid">
              <span class="skill-tag">HTML5</span>
              <span class="skill-tag">CSS3</span>
              <span class="skill-tag">JavaScript</span>
              <span class="skill-tag">Vue.js</span>
              <span class="skill-tag">Responsive Design</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AboutMe'
}
</script>

<style scoped>
.about-section {
  padding: 4rem 1rem;
  background-color: var(--surface);
  border-radius: 12px;
  margin: 2rem 0;
  width: 100%;
  box-sizing: border-box;
}

.about-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}

.section-title {
  text-align: center;
  margin-bottom: 2rem;
  color: var(--on-surface);
  font-size: 2.5rem;
}

.about-content {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  align-items: center;
}

.about-image {
  flex: 1;
  max-width: 300px;
  width: 100%;
}

.profile-pic {
  width: 100%;
  height: auto;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.about-text {
  flex: 2;
  color: var(--on-surface);
  line-height: 1.6;
}

.skills h3 {
  margin-top: 1.5rem;
  margin-bottom: 1rem;
  color: var(--primary);
}

.skills-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  margin-top: 0.5rem;
}

.skill-tag {
  background-color: rgba(187, 134, 252, 0.1);
  color: var(--primary);
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  border: 1px solid rgba(187, 134, 252, 0.2);
}

/* Tablet and larger */
@media (min-width: 768px) {
  .about-content {
    flex-direction: row;
    align-items: flex-start;
  }
  
  .about-image {
    margin-right: 2rem;
  }
}

/* Large desktops */
@media (min-width: 1024px) {
  .about-section {
    padding: 5rem 2rem;
  }
  
  .about-content {
    gap: 3rem;
  }
  
  .section-title {
    font-size: 3rem;
    margin-bottom: 3rem;
  }
}

/* Small mobile devices */
@media (max-width: 480px) {
  .about-section {
    padding: 2rem 0.5rem;
  }
  
  .section-title {
    font-size: 2rem;
    margin-bottom: 1.5rem;
  }
  
  .skill-tag {
    font-size: 0.8rem;
    padding: 0.4rem 0.8rem;
  }
}
</style>
