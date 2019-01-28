<template>
   <div>
       <div class="bg-1">
           <div class="work-progress">
               <div data-aos="slide-right"
                    data-aos-offset="200"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out" class="work-progress-info">
                   <h2>WORK <span>PROGRESS</span></h2>
                   <p>General steps we follow when working on project</p>
               </div>
               <div data-aos="slide-left"
                    data-aos-offset="200"
                    data-aos-duration="1000"
                    data-aos-easing="ease-in-out" class="work-progress-p">
                   <p>1.DISCUSS</p>
               </div>
               <div data-aos="slide-left"
                    data-aos-offset="200"
                    data-aos-duration="1050"
                    data-aos-easing="ease-in-out" class="work-progress-p">
                   <p>2.MAKE TARGETS</p>
               </div>
               <div data-aos="slide-left"
                    data-aos-offset="200"
                    data-aos-duration="1100"
                    data-aos-easing="ease-in-out" class="work-progress-p">
                   <p>3.DEVELOPEMENT</p>
               </div>
               <div data-aos="slide-left"
                    data-aos-offset="200"
                    data-aos-duration="1150"
                    data-aos-easing="ease-in-out" class="work-progress-p">
                   <p>4.PRODUCT</p>
               </div>
           </div>
       </div>
       <div class="bg-1">
           <div  class="some-work">
                <h2 data-aos="zoom-in-down"
                    data-aos-offset="200"
                    data-aos-duration="100"
                    data-aos-easing="ease-in-out">OUR SOME <span>WORK</span></h2>
                <p  class="info-2"><span>WE DEVELOPED</span> AWESOME STUFF</p>
               <p class="info-3">Following are the few samples of our work</p>
           </div>

       </div>
   </div>
</template>

<script>
    export default {
        name: "WorkProgress"
    }
</script>

<style scoped lang="scss">
    .bg-1{
        height: auto;
        width: 100%;
        background-image: url("../assets/bg1.jpg");
    }
    .work-progress{
        background-color: rgba(black,0.9);
        height: auto;
        padding-top: 10rem;
        padding-left: 8rem;
        display: flex;
        flex-wrap: wrap;
        padding-bottom: 12rem;

        & .work-progress-p{
            display: flex;
            flex-direction: column;
            margin: 2rem;
            justify-content: space-around;
            & p{
                color: #fff;
                font-family: sans-serif;
                font-size: 1.8rem;
                letter-spacing: 0.15rem;
            }
        }
        & h2{
              font-family: Roboto,sans-serif;
              font-size: 2.3rem;
              font-weight: 600;
              color: #fff;

        & span{
              font-size: inherit;
              font-family: inherit;
              color: #6aafca;
          }
        & ::after{
              content: '';
              display: block;
              height: 2px;
              width: 6.5rem;
              background-color: #efd282;
              margin: 1.3rem 0.5rem;
          }
    }

    &-info{
         font-family: sans-serif;
         color: #fff;
         font-size: 1.6rem;
         width: 25rem;
         font-weight: 300;
         line-height: 1.6;
         letter-spacing: 0.06rem;
     }
    }

    .some-work{
        background-color: rgba(255,255,255,0.9);
        height: inherit;
        display: flex;
        flex-direction: column;
        padding-top: 8rem;
        align-items: center;
        padding-bottom: 10rem;
        & h2{
            font-family: sans-serif;
            font-size: 3rem;
            font-weight: 800;
            color: #424242;
            & span{
                color: #6aafca;
                font-size: inherit;
            }
        }
        & .info-2{
            font-size: 1.4rem;
            letter-spacing: 0.1rem;
            font-family: sans-serif;
            font-weight: 600;
            color: #424242;
            margin:1.5rem 0;
            & span{
                color: #6aafca;
            }
        }

        & .info-3{
            color: #424242;
            font-size: 1.8rem;
            font-family: sans-serif;
            letter-spacing: 0.2rem;
            margin-top: 1rem;
        }

    }
</style>