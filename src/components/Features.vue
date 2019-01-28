<template>
    <div class="features">
        <div data-aos="flip-right"
             data-aos-offset="200"
             data-aos-duration="1000"
             data-aos-easing="ease-in-out" id="div-1">
            <img src="@/assets/logo.png" alt="">
            <strong>FULLY RESPONSIVE</strong>
            <p>KelcoTech is providing you web solutions with
                complete responsive solution across all devices and screens</p>
        </div>
        <div data-aos="flip-right"
             data-aos-offset="200"
             data-aos-duration="1000"
             data-aos-easing="ease-in-out" id="div-2">
            <img src="@/assets/logo.png" alt="">
            <strong>SEO FRIENDLY</strong>
            <p>KelcoTech is providing you web solutions with
                complete responsive solution across all devices and screens</p>
        </div>
        <div data-aos="flip-right"
             data-aos-offset="200"
             data-aos-duration="1000"
             data-aos-easing="ease-in-out" id="div-3">
            <img src="@/assets/logo.png" alt="">
            <strong>ONE & MULTI PAGE</strong>
            <p>KelcoTech is providing you web solutions with
                complete responsive solution across all devices and screens</p>
        </div>
        <div data-aos="flip-right"
             data-aos-offset="200"
             data-aos-duration="1000"
             data-aos-easing="ease-in-out" id="div-4">
            <img src="@/assets/logo.png" alt="">
            <strong>MARKETING MATERIALS</strong>
            <p>KelcoTech is providing you web solutions with
                complete responsive solution across all devices and screens</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Features"
    }
</script>

<style scoped lang="scss">
.features{
    display: flex;
    flex-wrap: wrap;
    & > div{
        display: flex;
        flex-grow: 1;
        flex-direction: column;
        align-items: center;
        font-family: Poppins,sans-serif;
        padding: 1rem;
        padding-top: 5rem;
        padding-bottom: 5rem;
        & strong{
            font-size: 2rem;
            font-weight: 600;
            letter-spacing: .3rem;
            margin-top: 2rem;
        }
        & p{
            text-align: center;
            max-width: 23.2vw;
            min-width: 30rem;
            margin-top: 3rem;
            line-height: 1.6;
        }
    }
    & #div-1,#div-3{
        background-color: #428ca8;
        color: #fff;
    }
    & #div-2,#div-4{
        background-color: #0f3f56;
        color: #fff;
    }
    & > div img{
        height: 8rem;
        width: 8rem;
    }
}
</style>