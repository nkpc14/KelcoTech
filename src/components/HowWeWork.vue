<template>
   <div class="bg">
       <div class="how">
           <h1 data-aos="slide-left"
               data-aos-offset="200"
               data-aos-duration="500"
               data-aos-easing="ease-in-out">HOW WE WORK</h1>
           <p data-aos="slide-up"
              data-aos-offset="200"
              data-aos-duration="1000"
              data-aos-easing="ease-in-out" class="info"><span>WE WORK WITH ALL OF OUR</span> DEDICATION</p>
           <p data-aos="slide-up"
              data-aos-offset="200"
              data-aos-duration="1000"
              data-aos-easing="ease-in-out" class="info-1">
               Our outstanding, virtual, dedicated and hardworking team
               is the backbone of Tech Code Solutions. They work in coordination
               and generate consonance which helps to overcome all the obstacles
               that come in the path of our customer to achieve their business objectives
           </p>
           <div class="how__items">
               <div data-aos="slide-right"
                    data-aos-offset="200"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out" class="how__items-1">
                   <div class="how__items-1-box"></div>
                   <h3>SELF-MOTIVATED TEAM</h3>
                   <p>We got awesome,experienced & hardworking team</p>
               </div>
               <div data-aos="slide-right"
                    data-aos-offset="200"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out" class="how__items-1">
                   <div class="how__items-1-box"></div>
                   <h3>INNOVATIVE</h3>
                   <p>We plan out the work on project with innovative ideas</p>
               </div>
               <div data-aos="slide-left"
                    data-aos-offset="200"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out" class="how__items-1">
                   <div class="how__items-1-box"></div>
                   <h3>CREATIVE</h3>
                   <p>We show our creativeness to make our clients happy</p>
               </div>
               <div data-aos="slide-left"
                    data-aos-offset="200"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out" class="how__items-1">
                   <div class="how__items-1-box"></div>
                   <h3>OVER-TIME</h3>
                   <p>We do over time for the project delivery if needed</p>
               </div>
           </div>
       </div>

   </div>
</template>

<script>
    export default {
        name: "HowWeWork"
    }
</script>

<style scoped lang="scss">
        .bg{
            background: url("../assets/bg2.jpg");
            z-index: 1000;
            height: auto;
            background-repeat: no-repeat;
            background-size: cover;
        }
        .how{
            font-family: Roboto,sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding-top: 8rem;
            background-color: rgba(255,255,255,0.9);
            z-index: 100;
            height: inherit;
            & h1{
                color: #424242;
                font-size: 4.1vw;
                line-height: inherit;
                margin-bottom: 1rem;
            }

            & .info{
                font-size: 1.6vw;
                font-weight: 500;
                letter-spacing: 0.04rem;
                margin-bottom: 2rem;
                color: #424242;
                & span{
                    color: #6aafca;
                    font-size: inherit;
                }
            }

            & .info-1{
                font-size: 1.6rem;
                color: #585858;
                max-width: 67rem;
                text-align: center;
                line-height: 1.6;
                margin-bottom: 8rem;
                padding:1rem ;
            }

            &__items{
                display: flex;
                flex-wrap: wrap;
                margin-bottom: 8rem;
                &-1{
                    height: 30rem;
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    align-content: space-around;
                    justify-content: space-around;
                    margin: auto;
                    &-box{
                        /*background-color: red;*/
                        height: 20rem;
                        width: 20rem;
                        border-radius: 100%;
                        border: solid 0.1rem;
                    }
                    & h3{
                        font-size: 1.5rem;
                        font-weight: 600;
                        margin-bottom: 1rem;
                        color: #555;
                        margin-top: 2rem;
                    }

                    & p{
                        font-family: inherit;
                        font-size: 1.4rem;
                        width: 25rem;
                        text-align: center;
                        letter-spacing: 0.15rem;
                        font-weight: 500;
                        line-height: 1.6;
                    }

                }
            }
        }

</style>