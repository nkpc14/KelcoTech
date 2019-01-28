<template>
   <div class="about-us">
       <img data-aos="fade-right"
            data-aos-offset="200"
            data-aos-duration="1000"
            data-aos-easing="ease-in-out"
            data-aos-mirror="true"
               src="../assets/services.png" alt="">
       <div  class="about-us__disc">
            <h1 data-aos="fade-down"
                data-aos-offset="200"
                data-aos-duration="1000"
                data-aos-easing="ease-in-out"
                data-aos-mirror="true"
            >ABOUT <span>US</span></h1>
           <p data-aos="fade-up"
              data-aos-offset="200"
              data-aos-duration="100"
              data-aos-easing="ease-in-out"
              data-aos-mirror="true"
                   class="about-us__disc--info"><span>WE PROVIDE</span> ONLINE SOLUTIONS</p>
           <p data-aos="fade-left"
              data-aos-offset="200"
              data-aos-duration="1000"
              data-aos-easing="ease-in-out"
              data-aos-mirror="true"
                   class="about-us__disc--info-1">" We are providing Software & Web Solutions, Implementation,
               Consulting Services and IT Trainings "</p>
           <p data-aos="fade-left"
              data-aos-offset="200"
              data-aos-duration="1000"
              data-aos-easing="ease-in-out"
              data-aos-mirror="true" class="about-us__disc--info-1">
               KelcoTech, is the leading information technology consulting, services,
               and business process outsourcing organization that envisioned and instigated
               the adoption of the flexible business practices that today enable our client
               companies to operate more efficiently and produce more value.
               KelcoTech’s strength lies in perceiving the client’s business processes,
               culture, vision and goals across the industry segments and offering client
               oriented solutions, which are highly reliable.
           </p>
       </div>
   </div>
</template>

<script>
    export default {
        name: "AboutUs"
    }
</script>

<style scoped lang="scss">
    .about-us{
        /*height: 80vh;*/
        width: 100%;
        display: flex;
        text-align: center;
        font-family: Poppins,sans-serif;
        flex-wrap: wrap;
        /*background-color: red;*/
        padding-top: 10rem;
        & img{
            width: 50vw;
            flex-grow: 1;
        }

        &__disc{
            /*background-color: green;*/
            display: flex;
            flex-direction: column;
            align-items: center;
            width: auto;
            flex-grow: 1;

            & h1{
                color: #424242;
                font-size: 4.1rem;
                line-height: inherit;
                font-weight: 800;
                & span{
                    color: rgba(#00b7ff,0.7);
                    font-size: inherit;
                    line-height: inherit;
                }
            }
            &--info{
                display: flex;
                justify-content: center;
                padding-top: 1rem;
                color: #424242;
                font-size: 1.6rem;
                line-height: 1.6;
                font-weight: 600;
                margin-bottom: 1rem;
                font-family:  Roboto,sans-serif;
                & span{
                    color: rgba(#00b7ff,0.7);
                    font-size: inherit;
                }
            }

            &--info-1{
                /*background-color: red;*/
                display: flex;
                justify-content: center;
                font-size: 1.6rem;
                line-height: 1.8;
                font-weight: 300;
                color: #585858;
                font-family: Roboto,sans-serif;
                margin-bottom: 2rem;
                max-width: 40rem;
            }

        }
    }
</style>