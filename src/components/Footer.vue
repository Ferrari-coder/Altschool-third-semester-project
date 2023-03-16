<template>
    <div class="container">
        <div class="line"></div>
        <div class="content">
            <p>Copyright <i class="fa-regular fa-copyright"></i> All rights reserved | This template is made by Aiyegbusi
                Oluwaferanmi</p>
            <div class="socials">

                <a href="mailto:oluwaferanmiaiyegbusi@gmail.com"><i class="fa-solid fa-envelope"></i></a>
                <a href="https://twitter.com/ahm_tamilore" target="_blank"><i class="fa-brands fa-twitter"></i></a>
                <a href="https://github.com/Ferrari-coder" target="_blank"><i class="fa-brands fa-github"></i></a>
                <a href="https://www.linkedin.com/in/oluwaferanmi-aiyegbusi-0952b4229/" target="_blank"><i
                        class="fa-brands fa-linkedin"></i></a>

            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: "FooterSection",
} 
</script>

<style lang="scss" scoped>
@use 'sass:math';

/* variables*/
$primary: #4D73F8;
$base-gap: 30px;
$text-color: #020C18;
$background: #ffffff;
$breakpoint-minipc: 1500px;
$breakpoint-tablet: 1350px;
$breakpoint-minitab: 900px;
$breakpoint-phone: 600px;
$breakpoint-miniphone: 500px;

.container {
    .line {
        border: 1px solid rgba(77, 115, 248, 0.15);
    }

    .content {
        display: flex;
        justify-content: space-between;
        align-items: center;

        p {
            font-size: 15px;
            color: #616161;
        }

        .socials {
            a {
                color: $primary;
                margin: 0 15px;
                font-size: 20px;
            }
        }

        @media(max-width: $breakpoint-minitab) {
            flex-direction: column;
            line-height: 24px;
            text-align: center;
        }
    }
}
</style>