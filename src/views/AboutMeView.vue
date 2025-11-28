<script setup>
import MainHeader from '@/components/MainHeader.vue'
import MainFooter from '@/components/MainFooter.vue'
</script>

<template>
  <main class="page">
    <MainHeader />

    <section class="page-content about-me">
      <h1>About me</h1>
      <p>I am a software developer specializing in creating solutions that improve the technical and operational efficiency of companies. I combine experience in <span>Python, C#, Angular, SQL, Docker, and Azure</span> with a strong focus on process automation and cloud application development.</p>
      <p>Throughout my career, I have designed and implemented <span>automated tools, CI/CD pipelines, and cloud applications</span> that have optimized workflows and enhanced collaboration in demanding environments. I am motivated to build software that truly adds value, solving problems in an elegant and scalable way.</p>
      <p>I currently work as a <span>Principal Software Developer</span>, where I lead advanced technical solutions, manage infrastructure in <span>Azure and Autodesk Platform Services</span>, and contribute to improving the integration and productivity of multidisciplinary teams.</p>
      <p>At the same time, I continue to train in areas such as <span>Artificial Intelligence</span>, keeping up to date with emerging technologies to continue growing professionally.</p>
      <p>I am a curious, results-oriented person who is passionate about transforming ideas into tools that make a difference.</p>
      <h2>Pedro Rizquez</h2>
      <h3>Passionate about building efficient solutions through code</h3>
    </section>

    <MainFooter />
  </main>
</template>

<style scoped>
.about-me {
  padding: 0px 300px;
}

p, li {
  font-size: 1.3rem;
  color: var(--text-100);
  text-align: justify;
  font-weight: lighter;
}

ul li::marker {
  color: var(--text-100);
}

h1, h2 {
  color: var(--primary-100);
}

h1 {
  font-weight: 500;
  font-size: 2.5rem;
  text-align: center;
}

h2 {
  font-weight: lighter;
  font-size: 1.8rem;
  text-align: right;
}

h3 {
  font-size: 1.4rem;
  font-style: oblique;
  color: var(--primary-200);
  text-align: right;
  font-weight: lighter;
}

span {
  font-weight: 500;
}

@media (max-width: 1600px) {
  .about-me {
    padding: 0px 200px;
  }
}

@media (max-width: 1200px) {
  .about-me {
    padding: 0px 80px;
  }
}

@media (max-width: 768px) {
  .about-me {
    padding: 0px 30px;
  }

  h1 {
    font-size: 2.3rem;
  }

  h2 {
    font-size: 1.6rem;
  }

  h3 {
    font-size: 1.2rem;
  }

  p, li {
    font-size: 0.95rem;
  }
}

@media (max-width: 480px) {
  .policy {
    padding: 0px 30px;
  }

  h1 {
    font-size: 2.1rem;
  }

  h2 {
    font-size: 1.4rem;
  }

  h3 {
    font-size: 1rem;
  }

  p, li {
    font-size: 0.9rem;
  }
}
</style>