<template>
<div>
    <LearningFieldsCards :LearningFields="LearningFields" />
    <TrustedName />
    <SectionEmpower />
    <SectionTestimonials />
    <SectionArticle />
    <SectionPopularPlans :PopularPlans="PopularPlans" />
    <SectionPricingPlans />
    <SectionPartners />
</div>
</template>

<script>
import LearningFieldsCards from './LearningFieldsCards.vue';
import TrustedName from './TrustedName.vue';
import SectionEmpower from './SectionEmpower.vue'
import SectionTestimonials from './SectionTestimonials.vue';
import SectionArticle from './SectionArticle.vue';
import SectionPopularPlans from './SectionPopularPlans.vue';
import SectionPricingPlans from './SectionPricingPlans.vue';
import SectionPartners from './SectionPartners.vue';
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
            ],

            PopularPlans:[
                {
                    title: 'Android Developer',
                    imgUrl: 'android-developer',
                    teacher: 'David Sanders',
                    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus nam repellat ex animi ipsam fugit recusandae officiis provident officia esse!',
                    numberOfPeople: '1',
                    field: 'Programming',
                    id: 1,
                },
                {
                    title: 'Web Design',
                    imgUrl: 'web-design',
                    teacher: 'Jennifer Powell',
                    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus nam repellat ex animi ipsam fugit recusandae officiis provident officia esse!',
                    numberOfPeople: '1',
                    field: 'Programming',
                    id: 2,
                },
                {
                    title: 'Financial Modeling',
                    imgUrl: 'financial-modeling',
                    teacher: 'Edward Bowman',
                    description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus nam repellat ex animi ipsam fugit recusandae officiis provident officia esse!',
                    numberOfPeople: '1',
                    field: 'Business',
                    id: 3,
                },

            ]
        };
        
    },
    components: {
    LearningFieldsCards,
    TrustedName,
    SectionEmpower,
    SectionTestimonials,
    SectionArticle,
    SectionPopularPlans,
    SectionPricingPlans,
    SectionPartners
}
}
</script>

<style scoped lang="scss">

</style>
