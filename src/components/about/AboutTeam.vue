<template>
  <div class="container my-5">
            <div class="row mb-4">
                <div class="col-12">
                    <div class="section-title text-center">
                        <h2 class="title">Our members</h2>
                        <p class="sub-title">With young talents, the king of coders, the destroyer of Front-End!</p>
                    </div>
                </div>
            </div>

            <div class="row mb-n6 justify-content-center">
                <div class="col-lg-3 col-md-4 col-sm-6" v-for="(item, index) in members" :key="index">
                    <div class="single-team-member text-center mb-6">
                        <div class="team-thumb">
                            <img class="fit-image" :src="item.img" alt="Team Image">
                            <div class="team-social">
                                <a :href="item.linkFb" target="_blank">
                                    <b-icon icon="facebook"></b-icon>
                                </a>
                                <a href="#"><b-icon icon="linkedin"></b-icon></a>
                                <a href="#"><b-icon icon="twitter"></b-icon></a>
                            </div>
                        </div>
                        <div class="team-content">
                            <h6 class="team-member-name">{{item.name}}</h6>
                            <p>{{item.role}}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name: 'AboutTeam',
    data() {
        return {
            members: [
                {
                    img: require("@/assets/images/about/member1.jpg"),
                    role: 'Developer',
                    name: 'Tú Xuân',
                    linkFb: 'https://www.facebook.com/tucute200/'
                },
                {
                    img: require("@/assets/images/about/member2.jpg"),
                    role: 'Designer',
                    name: 'Lê Văn Phong',
                    linkFb: 'https://www.facebook.com/phong.levan.5815255'
                },
                 {
                    img: require("@/assets/images/about/member3.jpg"),
                    role: 'Developer',
                    name: 'Võ Hoàng Long',
                    linkFb: 'https://www.facebook.com/longrui.09'
                },
            ]
        }
    }
}
</script>

<style scoped src="@/assets/css/components/about/AboutTeam.css">

</style>