<template>
    <div class="main-container">
        <ProfileSection />
        <RepoSection />
        <FooterSection />
    </div>
</template>
  
<script>
import ProfileSection from './Profile.vue'
import RepoSection from './Repos.vue'
import FooterSection from './Footer.vue';

export default {
    name: 'HomePage',
    components: {
        ProfileSection,
        RepoSection,
        FooterSection
    }
}
</script>
  
<style lang="scss" scoped>


</style>