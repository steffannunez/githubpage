<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Education</template>
      <p>Ingeniering Science Degree</p> 
      <p>Graduate in Computer and Informatics Execution Engineering</p> 
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Experience</template>
      <p>Back-end developer, UrbanCoop, 2020</p>
      <p>Full stack Developer, Tenlove Spa, 2021-2022</p>
      <p>Software Developer, Talana linQ Spa, 2022 - present</p>
      <p>FullStack Developer, proyectos personales, 2016 - present</p>
      

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Skills</template>
    <h3  class="miniTitle">Programming Languages:</h3>
    <p> Java, Python, JavaScript, C#, Dart, Kotlin, Swift</p>
    <h3 class="miniTitle">Web Development:</h3>
    <p> HTML, CSS, SCSS, Vue.js, JavaScript, TypeScript, Node.js</p>
    <h3 class="miniTitle">Database Management:</h3>
    <p> PostgreSQL, MongoDB, MySQL, GoogleCloud</p>
    <h3 class="miniTitle">Software Development Tools:</h3>
    <p> Git, Eclipse, Visual Studio, IntelliJ IDEA, Android Studio, Xcode</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <!-- <template #heading>Projects</template>
    You can review my projects on
    <a class="githublink" href="https://github.com/steffannunez/" target="_blank" rel="noopener">GitHub</a>
     -->
     <template #heading> Hobbies</template>
      <p>-Drawing and reading Manga</p>
      <p>-Studying Physics and Programming</p>
      <p>-Collecting Figures and Perfumes</p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Habilidades</template>
    <p>Español (nativo)</p>
    <p>Intermediate/Advanced English</p>
    <p>Basic Italian</p>
    
  </WelcomeItem>
</template>

<style>
.miniTitle{
  color: rgb(238, 238, 238);
}
a{
  color: #008ab4;
}
a:hover{
  background: transparent;
  color: #d09effd2;
}
.githublink{
  color: #8100b4;
}
</style>