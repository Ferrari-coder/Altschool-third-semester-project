<template>
    <div class="container">
        <!-- v-for="profile in data" :key="profile.id" -->
        <div class="image"><img src="https://avatars.githubusercontent.com/u/73191967?v=4" alt="avi" /></div>
        <div class="profile-content">
            <h2>{{data.name}}</h2>
            <p>@{{data.login}}</p>
            <h5>Front-End Engineer</h5>
            <section class="section">
                <div class="stat" id="repos">
                    <p class="profile-figures" id="repo-fig">{{data.public_repos}}</p>
                    <h3 class="profile-details"> Repositories</h3>
                </div>
                <div class="stat">
                    <p class="profile-figures">{{ data.followers }}</p>
                    <h3 class="profile-details"> Followers</h3>
                </div>
                <div class="stat">
                    <p class="profile-figures">{{data.following}}</p>
                    <h3 class="profile-details">Following</h3>
                </div>
                <!-- <div class="socials">
                    <h3>Get In Touch:</h3>
                    <div class="icons">
                        <a href="mailto:oluwaferanmiaiyegbusi@gmail.com"><i class="fa-solid fa-envelope"></i></a>
                        <a href="https://twitter.com/ahm_tamilore" target="_blank"><i class="fa-brands fa-twitter"></i></a>
                        <a href="https://github.com/Ferrari-coder" target="_blank"><i class="fa-brands fa-github"></i></a>
                        <a href="https://www.linkedin.com/in/oluwaferanmi-aiyegbusi-0952b4229/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                    </div>
                </div> -->
            </section>
        </div>
    </div>
</template>

<script>
import axios from "axios"
export default {
    name: 'ProfileSection',
    data() {
        return {
            data: "",
        };
    },
    mounted() {
        axios.get("https://api.github.com/users/Ferrari-coder")
            .then(response => response.data)
            .then((data) => {this.data = data; })
            // console.log(data)
    }
}
</script>

<style lang="scss" scoped>
@use 'sass:math';

/* variables*/
$primary: #4D73F8;
$base-gap: 30px;
$text-color: #020C18;
$background: #ffffff;
$breakpoint-minipc:1500px;
$breakpoint-tablet:1350px;
$breakpoint-minitab:800px;
$breakpoint-phone:600px;
$breakpoint-miniphone:500px;

.container {
    display: flex;
    gap: $base-gap;
    align-items: center;
    background: rgba(77, 115, 248, 0.03);
    border: 1px solid rgba(77, 115, 248, 0.15);
    padding: $base-gap;
    border-radius: $base-gap/3;


    .image {
        width: 222px;
        height: 222px;
        padding: 5px;
        position: relative;
        border-radius: 50%;
        background: linear-gradient(to bottom, rgba(77, 115, 248, 1), rgba(77, 115, 248, 0.15));

        img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
        }
    }

    .profile-content {
        line-height: 15px;

        h2 {
            font-family: 'Merriweather';
            font-style: normal;
            font-weight: 700;
            font-size: 30px;
            color: $text-color;
        }

        p {
            font-weight: 400;
            font-size: 16px;
            color: #616161;
            font-family: 'Roboto';
            line-height: 10px;
        }

        h5 {
            font-weight: 600;
            font-size: 20px;
            color: $text-color;
            line-height: 10px;
        }

        .section {
            display: flex;
            gap: $base-gap;

            .stat {
                padding: $base-gap/3;
                width: 150px;
                background: rgba(77, 115, 248, 0.2);
                border-radius: 4px;
                text-align: center;
                line-height: $base-gap/3;
            }

        //     .socials {}
        }
    }
}
</style>