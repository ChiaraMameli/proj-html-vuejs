<template>
<div>
    <LearningFieldsCards :LearningFields="LearningFields" />
    <TrustedName />
    <SectionEmpower />
    <SectionTestimonials />
    <SectionArticle />
</div>
</template>

<script>
import LearningFieldsCards from './LearningFieldsCards.vue';
import TrustedName from './TrustedName.vue';
import SectionEmpower from './SectionEmpower.vue'
import SectionTestimonials from './SectionTestimonials.vue';
import SectionArticle from './SectionArticle.vue';
export default {
    name: "BaseMain",
    data() {
        return {
            LearningFields: [
                {
                    label: "languages",
                    imgUrl: "globe",
                    id: 1,
                },
                {
                    label: "software",
                    imgUrl: "pen",
                    id: 2,
                },
                {
                    label: "business",
                    imgUrl: "case",
                    id: 3,
                },
                {
                    label: "chemistry",
                    imgUrl: "test-tubes",
                    id: 4,
                },
                {
                    label: "science",
                    imgUrl: "rocket",
                    id: 5,
                },
                {
                    label: "DIY&Craft",
                    imgUrl: "scissors",
                    id: 6,
                },
            ]
        };
    },
    components: { LearningFieldsCards, TrustedName, SectionEmpower, SectionTestimonials, SectionArticle }
}
</script>

<style scoped lang="scss">

</style>
