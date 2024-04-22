<template>
    <div>
        <!-- <p class="text-xs mb-5 text-theme-secondary text-center">Let's stay connected:</p> -->
        <div class="flex justify-center">
            <a href="https://www.linkedin.com/in/rodrigo-castro-velazquez/" target="_blank"><linkedin-icon size="1.5x" class="mr-3"></linkedin-icon></a>
            <a href="https://github.com/snowtxc" target="_blank"><github-icon size="1.5x" class="mr-3"></github-icon></a>
        </div>

    </div>
</template>

<script>
import { TwitterIcon, LinkedinIcon, GithubIcon  } from 'vue-feather-icons'

export default {
  components: {
    TwitterIcon,
    LinkedinIcon,
    GithubIcon,
  }
}
</script>
