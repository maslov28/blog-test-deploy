<template>
  <div>
    <start-section></start-section>
    <benefits-section></benefits-section>
    <adventages-section></adventages-section>
    <competencies-section></competencies-section>
    <comparison-section></comparison-section>
    <projects-section></projects-section>
    <feedback-section></feedback-section>
    <discussion-section></discussion-section>
    <footer-section></footer-section>
  </div>
</template>

<script>
import StartSection from '@/components/blocks/start-section/StartSection.vue'
import BenefitsSection from '@/components/blocks/benefits-section/BenefitsSection.vue'
import AdventagesSection from '@/components/blocks/adventages-section/AdventagesSection.vue'
import CompetenciesSection from '@/components/blocks/competencies-section/CompetenciesSection.vue'
import ComparisonSection from '@/components/blocks/comparison-section/ComparisonSection.vue'
import ProjectsSection from '@/components/blocks/projects-section/projects-section.vue'
import FeedbackSection from '@/components/blocks/feedback-section/feedback-section.vue'
import DiscussionSection from '@/components/blocks/discussion-section/discussion-section.vue'
import FooterSection from '@/components/blocks/footer/footer-section.vue'

export default {
  components: {
    StartSection,
    BenefitsSection,
    AdventagesSection,
    CompetenciesSection,
    ComparisonSection,
    ProjectsSection,
    FeedbackSection,
    DiscussionSection,
    FooterSection
  }
}
</script>

<style lang="scss">

</style>
