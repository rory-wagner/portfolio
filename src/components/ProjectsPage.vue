<template>
  <div id="projectsPage" class="projects-page">
    <div class="projects-header-div">
      <h1>Projects</h1>
    </div>

    <div class="projects-grid">
      <div
        v-for="(project, index) in projects"
        :key="index"
        class="project-card"
      >
        <component
          :is="project.link ? 'a' : 'div'"
          v-bind="project.link ? {
            href: project.link,
            target: '_blank',
            rel: 'noopener noreferrer',
          } : {}"
          :class="{ 'card-screenshot-link': project.link }"
        >
          <div class="card-screenshot">
            <img
              v-if="project.image"
              :src="project.image"
              :alt="project.title + ' screenshot'"
              loading="lazy"
              decoding="async"
              class="card-img"
            />
            <div v-else class="card-img-placeholder">
              <span>No Screenshot</span>
            </div>
          </div>
        </component>

        <div class="card-body">
          <h2 class="card-title">{{ project.title }}</h2>
          <p class="card-description">{{ project.description }}</p>

          <div v-if="project.tags && project.tags.length" class="card-tags">
            <span
              v-for="tag in project.tags"
              :key="tag"
              class="tag"
            >{{ tag }}</span>
          </div>

          <div class="card-links">
            <a
              v-if="project.link"
              :href="project.link"
              target="_blank"
              rel="noopener noreferrer"
              class="card-btn primary"
            >View Project</a>
            <a
              v-if="project.repo"
              :href="project.repo"
              target="_blank"
              rel="noopener noreferrer"
              class="card-btn secondary"
            >Source Code</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProjectsPage',
  data() {
    return {
      projects: [
        {
          title: 'Finding Mom',
          description: 'Top down video game made in Godot. The game can be downloaded from Steam.',
          image: require('@/assets/FindingMomThumbnail.png'),
          link: 'https://store.steampowered.com/app/3560500/Finding_Mom/',
          repo: 'https://github.com/rory-wagner/finding_mom',
          tags: ['Godot', 'GDScript'],
        },
        {
          title: 'DPM',
          description: 'A simple password manager that uses a deterministic algorithm to generate passwords based on a master password and a site name.',
          image: require('@/assets/DPMScreenshot.png'),
          repo: 'https://github.com/rory-wagner/dpm',
          tags: ['Python', 'Cryptography'],
        },
        {
          title: 'Ecommerce Website',
          description: 'Coming Soon!',
          tags: ['Golang', 'Vue', 'PostgreSQL'],
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import './../assets/variables.scss';

.projects-page {
  padding: 28px;
  margin-top: 2rem;
  margin-bottom: 2rem;
  background: rgba(255, 255, 255, 0.02);
  border-radius: 12px;
  box-shadow: 0 6px 18px rgba(2, 6, 23, 0.6);
  box-sizing: border-box;
}

.projects-header-div {
  text-align: center;
  margin-bottom: 2rem;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
}

.project-card {
  background: var(--glass);
  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 10px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  transition: transform 0.2s ease, box-shadow 0.2s ease;

  &:hover {
    transform: translateY(-4px);
    box-shadow: 0 10px 28px rgba(2, 6, 23, 0.7);
  }
}

.card-screenshot-link {
  display: block;
}

.card-screenshot {
  width: 100%;
  aspect-ratio: 16 / 9;
  overflow: hidden;
  background: rgba(0, 0, 0, 0.3);
}

.card-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transition: transform 0.3s ease;

  .project-card:hover & {
    transform: scale(1.04);
  }
}

.card-img-placeholder {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: $muted-slate;
  font-size: 0.875rem;
  letter-spacing: 0.05em;
}

.card-body {
  padding: 16px 20px 20px;
  display: flex;
  flex-direction: column;
  flex: 1;
}

.card-title {
  font-size: 1.15rem;
  margin: 0 0 8px;
  color: var(--ivory);
}

.card-description {
  font-size: 0.9rem;
  color: $muted-slate;
  line-height: 1.55;
  flex: 1;
  text-align: initial;
  margin: 0 0 14px;
}

.card-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  margin-bottom: 14px;
}

.tag {
  font-size: 0.75rem;
  padding: 3px 10px;
  border-radius: 20px;
  background: rgba(255, 107, 102, 0.15);
  color: $accent-coral;
  border: 1px solid rgba(255, 107, 102, 0.3);
  letter-spacing: 0.03em;
}

.card-links {
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
}

.card-btn {
  display: inline-block;
  padding: 7px 18px;
  border-radius: 6px;
  font-size: 0.85rem;
  font-weight: 600;
  text-decoration: none;
  transition: opacity 0.15s ease, background 0.15s ease;

  &.primary {
    background: $accent-coral;
    color: #fff;

    &:hover {
      opacity: 0.85;
    }
  }

  &.secondary {
    background: transparent;
    color: $accent-coral;
    border: 1px solid $accent-coral;

    &:hover {
      background: rgba(255, 107, 102, 0.12);
    }
  }
}

@media screen and (max-width: 800px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }
}
</style>
