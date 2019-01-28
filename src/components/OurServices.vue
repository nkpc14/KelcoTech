<template>
    <div class="our-services">
        <h2>OUR <span>SERVICES</span></h2>
        <p>Our team is committed to provide IT Services with :
            <span>Quality</span> | <span>Technology</span> | <span>Innovation</span>
        </p>
        <div data-aos="zoom-in"
             data-aos-offset="200"
             data-aos-duration="1000"
             data-aos-easing="ease-in-out-cubic"
             data-aos-mirror="true" class="grid">
            <div class="grid__box">
                <h4>Web Designing</h4>
                <p>We Design with Quality Solutions</p>
            </div>
            <div class="grid__box">
                <h4>Web Development</h4>
                <p>We Build Brands with Quality Solutions</p>
            </div>
            <div class="grid__box">
                <h4>SEO Internet Marketing</h4>
                <p>Increase your ranking in search results</p>
            </div>
            <div class="grid__box">
                <h4>Mobile Applications</h4>
                <p>Content Writing</p>
            </div>
            <div class="grid__box">
                <h4>Content Writing</h4>
                <p>Provide professional contents for your website</p>
            </div>
            <div class="grid__box">
                <h4>E-Learning</h4>
                <p>Provide highly interactive web based training</p>
            </div>
            <div class="grid__box">
                <h4>ORM</h4>
                <p>Promote positive content to the top of your search results</p>
            </div>
            <div class="grid__box">
                <h4>Finance & Accounts</h4>
                <p>Maintaining the revenue & expenses of your business</p>
            </div>
            <div class="grid__box">
                <h4>Logo Designing</h4>
                <p>Give your company a brand symbol</p>
            </div>
            <div class="grid__box">
                <h4>Video Presentation</h4>
                <p>Make videos for marketing purpose</p>
            </div>
            <div class="grid__box">
                <h4>Digital Marketing</h4>
                <p>Increase your business ranking in the digital world</p>
            </div>
            <div class="grid__box">
                <h4>Virtual Assistance</h4>
                <p>get personal assistance for your new startup</p>
            </div>

        </div>
    </div>
</template>

<script>
    export default {
        name: "OurServices"
    }
</script>

<style scoped lang="scss">
    .our-services{
        background-color: rgba(black,0.9);
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 7rem;
        & h2{
            font-size: 2vw;
            font-family: Roboto,sans-serif;
            font-weight: 800;
            color: #fff;
            & span{
                font-size: inherit;
                color: rgba(#00b7ff,0.8);
                font-family: inherit;
            }

            & ::after{
                content: '';
                display: block;
                height: 2px;
                width: 5vw;
                background-color: #efd282;
                margin: 1.3rem auto 1.8rem;
            }
        }

        & p{
            font-family: Roboto,sans-serif;
            margin-top: 1rem;
            font-size: 1.5vw;
            margin-bottom: 7rem;
            /*letter-spacing: 0.1rem;*/
            color: #fff;
            & span{
                /*letter-spacing: inherit;*/
                font-size: inherit;
                color: #efd282;
            }
        }


        & .grid{
            display: flex;
            margin: 0 10rem;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
            margin-bottom: 7rem;

            &__box{
                width: 25rem;
                background-color: red;
                height: 22rem;
                margin: 1rem;
                background-color: rgba(13,94,134,.3607843137254902);
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                & h4{
                    color: #fff;
                    font-size: 2rem;
                    font-weight: 400;
                    margin-top: 1rem;
                    margin-bottom: 1rem;
                    font-family: Roboto,sans-serif;
                }
                & p{
                    color: #c5c5c5;
                    font-size: 1.4rem;
                    line-height: 2.5rem;
                    letter-spacing: 0.09rem;
                    text-align: center;
                    width: 20rem;
                }
            }
        }
    }
</style>