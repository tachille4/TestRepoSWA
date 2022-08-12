<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>About Me</template>

    Learn more about my background, experiences, and interests. 
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>My Projects</template>

    Read more about what I have created for the world. 
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Get In Touch</template>

    Reach me via <a href="mailto:staticwebapps@outlook.com">email</a> or 
    <a target="_blank" href="https://twitter.com/AzureStaticApps">@AzureStaticApps</a>. 
    I'd love to learn more about how to improve your developer experience!
  </WelcomeItem>
</template>
