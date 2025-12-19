<script setup>
import MainHeader from '@/components/MainHeader.vue';
import MainFooter from '@/components/MainFooter.vue';
import Project from '@/components/Project.vue';

import common from '@/assets/images/png/Common.png';
import a_start from '@/assets/images/png/a_star.png';

/**
 * Object containing Codemnesis project information.
 * 
 * @property {string} title        Project name.
 * @property {string} imgSrc       Path or import of the representative image.
 * @property {string} imgAlt       Alternative text for the image (accessibility).
 * @property {string} description  General description of the project.
 * @property {string} technologies Technologies used in the project.
 * @property {string} note         Explanatory note or project status.
 * @property {string} linkLabel    Text of the link to access the resource.
 * @property {string} linkHref     URL of the external resource (e.g., repository).
 */
const codemnesis = {
  title: 'Codemnesis',
  imgSrc: common,
  imgAlt: 'Common app logo',
  description: 'Codemnesis is a tool that automatically analyzes code repositories to generate clear and useful documentation. Its goal is to save developers time by automatically creating files such as README, flowcharts, and explanations of each module, without relying on manual writing.',
  technologies: 'Python',
  note: 'This project is currently under development and is ready to be executed through the console terminal.',
  linkLabel: 'Browse the repository',
  linkHref: 'https://github.com/Rizquez/Codemnesis'
}

/**
 * Object containing A* project information.
 * 
 * @property {string} title        Project name.
 * @property {string} imgSrc       Path or import of the representative image.
 * @property {string} imgAlt       Alternative text for the image (accessibility).
 * @property {string} description  General description of the project.
 * @property {string} technologies Technologies used in the project.
 * @property {string} note         Explanatory note or project status.
 * @property {string} linkLabel    Text of the link to access the resource.
 * @property {string} linkHref     URL of the external resource (e.g., repository).
 */
const a_star_algorithm = {
  title: 'A* Algorithm',
  imgSrc: a_start,
  imgAlt: 'Common app logo',
  description: 'The A* algorithm is widely used due to its ability to find optimal paths efficiently, combining uniform cost search with informed heuristics to improve performance.',
  technologies: 'Python',
  note: 'This project is educational in nature and serves to understand the basic principles and applications of the A* search algorithm.',
  linkLabel: 'Browse the repository',
  linkHref: 'https://github.com/Rizquez/a-star-algorithm'
}
</script>

<template>
  <main>
    <MainHeader />

    <section>
      <h1>Personal projects</h1>
      <div class="projects">
        <Project v-bind="codemnesis" />
      </div>
    </section>

    <hr class="horizontal-line" />

    <section>
      <h1>Learning projects</h1>
      <div class="projects">
        <Project v-bind="a_star_algorithm" />
      </div>
    </section>

    <MainFooter />
  </main>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.5rem;
  text-align: center;
  color: var(--primary-100);
  margin-bottom: 0;
  padding-top: 20px;
}

.projects {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  gap: 2rem;
  flex-wrap: wrap;
  padding: 50px 0px;
}

@media (max-width: 1000px) {
  .projects {
    padding: 40px 60px;
  }

  h1 {
    font-size: 2.3rem;
  }
}

@media (max-width: 768px) {
  .projects {
    padding: 30px 40px;
    flex-direction: column;
    align-items: center;
  }

  h1 {
    font-size: 2rem;
  }
}

@media (max-width: 480px) {
  .projects {
    padding: 20px;
  }

  h1 {
    font-size: 1.8rem;
  }
}
</style>