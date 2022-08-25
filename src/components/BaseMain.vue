<template>
<main>
    <SectionFieldsCards :Fields="Fields" />
    <SectionIntroduction />
    <SectionEmpower />
    <SectionTestimonials />
    <SectionArticle />
    <SectionPopularPlans :PopularPlans="PopularPlans" />
    <SectionPricingPlans :PricingPlans="PricingPlans" />
    <SectionPartners :Partners="Partners" />
</main>
</template>

<script>
import SectionFieldsCards from './SectionFieldsCards.vue';
import SectionIntroduction from './SectionIntroduction.vue';
import SectionEmpower from './SectionEmpower.vue'
import SectionTestimonials from './SectionTestimonials.vue';
import SectionArticle from './SectionArticle.vue';
import SectionPopularPlans from './SectionPopularPlans.vue';
import SectionPricingPlans from './SectionPricingPlans.vue';
import SectionPartners from './SectionPartners.vue';
export default {
    name: "BaseMain",
    components: {
    SectionFieldsCards,
    SectionIntroduction,
    SectionEmpower,
    SectionTestimonials,
    SectionArticle,
    SectionPopularPlans,
    SectionPricingPlans,
    SectionPartners,
},
    data() {
        return {
            Fields: [
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

            ],

            PricingPlans: [
                {
                    id: 1,
                    imgUrl:'brain',
                    label: 'Standard',
                    price: '$12',
                    numberOfCourses: '2',
                    time: '15 Days',
                    webDesigning: true,
                    humanCenteredDesign: true,
                    basicMarketing: false,
                    phyton: false,
                    androidDeveloper: false,
                    businessEnglish: false,
                },
                {
                    id: 2,
                    imgUrl:'bulb',
                    label: 'Professional',
                    price: '$59',
                    numberOfCourses: '4',
                    time: '30Days',
                    webDesigning: true,
                    humanCenteredDesign: true,
                    basicMarketing: true,
                    phyton: true,
                    androidDeveloper: false,
                    businessEnglish: false,
                },
                {
                    id: 3,
                    imgUrl:'hat',
                    label: 'Advanced',
                    price: '$88',
                    numberOfCourses: '6',
                    time: '30 Days',
                    webDesigning: true,
                    humanCenteredDesign: true,
                    basicMarketing: true,
                    phyton: true,
                    androidDeveloper: true,
                    businessEnglish: true,
                },

            ],

            Partners:[
                {
                    id: 1,
                    label: 'Teach Hub',
                    imgUrl: 'teach-hub',
                    link: '#',
                },
                {
                    id: 2,
                    label: 'Study Central',
                    imgUrl: 'study-central',
                    link: '#',
                },
                {
                    id: 3,
                    label: 'Educator',
                    imgUrl: 'educator',
                    link: '#',

                },
                {
                    id: 4,
                    label: 'Scholar',
                    imgUrl: 'scholar',
                    link: '#',

                },
            ]
        };
        
    },
}
</script>

<style scoped lang="scss">
</style>
