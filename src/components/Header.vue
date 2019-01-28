<template>
<div  class="header">

        <div  class="header__main">
            <img src="../assets/logo.png" alt="logo">
            <ul v-if="displayHeader"
                data-aos="slide-left"
                data-aos-offset="200"
                data-aos-duration="1000"
                data-aos-easing="ease-in-out">
                <li><a href="">HOME</a></li>
                <li><a href="">ABOUT</a></li>
                <li><a href="">PROJECTS</a></li>
                <li><a href="">SERVICES</a></li>
                <li><a href="">PORTFOLIO</a></li>
                <li><a href="">CAREERS</a></li>
                <li><a href="">CONTACT</a></li>
            </ul>
            <a  @click="displayHeader = !displayHeader" class="drawer"><img src="../assets/drawer.png" alt=""></a>
        </div>
    <div  class="header__inner">
        <div >
            <h1 data-aos="fade-up"
                data-aos-offset="200"
                data-aos-delay="50"
                data-aos-duration="1000"
                data-aos-easing="ease-in-out"
                data-aos-mirror="true"
            >
                KELCO<span>TECH</span>
            </h1>
            <p >A Perfect Way To Start Your Business Online</p>
            <button  id="get-started">GET STARTED</button>
        </div>
    </div>


    <vue-particles
            color="#fff"
            :particleOpacity="0.7"
            :particlesNumber="80"
            shapeType="circle"
            :particleSize="3"
            linesColor="#13E8E9"
            :linesWidth="2"
            :lineLinked="true"
            :lineOpacity="0.1"
            :linesDistance="150"
            :moveSpeed="2"
            :hoverEffect="true"
            hoverMode="grab"
            :clickEffect="true"
            clickMode="push">

    </vue-particles>
</div>
</template>

<script>
    export default {
        name: "Header",
        data () {
            return {
                displayHeader: false,
                width: 0,
            };
        },
        created() {
            window.addEventListener('resize', this.handleResize)
            this.handleResize();
        },
        destroyed() {
            window.removeEventListener('resize', this.handleResize)
        },
        methods: {
            handleResize() {
                this.width = window.innerWidth;
                console.log(this.width);
                if (this.displayHeader===false && this.width>=920){
                    this.displayHeader=true
                }
                else {
                    this.displayHeader=false
                }
            },
        }


    }
</script>

<style scoped lang="scss">
    .displayNone{
        display: none;
    }
    #particles-js{
        position: absolute;
        top: 0;
        left: 0;
        height: 99vh;
        width: 100%;
        z-index: 0;
    }
    .header{
        height: 100vh;
        width: 100%;
        background-image: url("../assets/bgn22.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        & .drawer{
            z-index: 1000;
            display: none;
            position: fixed;
            right: 4rem;
            & img{
                z-index: 1000;
                height: 4rem;
                width: 4rem;
                margin-right: 4vw;
                cursor: pointer;
            }
            @media only screen and (max-width:920px) {
                display: block;
            }
        }
        &__main ul{
            margin-right: 2rem;
            z-index: 1000;
            @media only screen and (max-width: 920px){
                position: fixed;
                right: -5.5vw;
                display: flex;
                flex-wrap: wrap;
                flex-direction: column;
                background-color: #424242;
                width: 40vw;
                height: 72vh;
                margin-top: 42vh;
                padding-top: 20rem;
                padding-right: 2rem;
            }
        }
        &__main ul > li{
            z-index: 1000;
            float: left;
            display: block;
            margin-left: 3.5rem;
            font-family: Poppins,sans-serif;
            @media only screen and (max-width: 920px){
                /*display: none;*/
                display: flex;
                flex-wrap: wrap;
                flex-direction: column;
                padding: 2rem;
                justify-content: center;
                align-items: center;
            }
        }
        &__main ul > li a{
            text-decoration: none;
            color: #fff;
            font-weight: 500;
        }
        &__main{
            /*background-color: red;*/
            font-size: 1.4rem;
            float: left;
            display: flex;
            align-items: center;
            justify-content: space-between;
            height: 9rem;
            width: 100%;

            & img {
                height: 8rem;
                margin-left: 6vw;
                margin-top: 2rem;
                z-index: 1000;
            }
        }

        &__inner{
            background-color: rgba(black,0.9);
            position: relative;
            height: 100vh;
            & div{
                /*background-color: red;*/
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                min-width: 90%;
                & h1{
                    font-size: 4.5vw;
                    font-family: Roboto,sans-serif;
                    font-weight: 900;
                    letter-spacing: 0.5rem;
                    line-height: initial;
                    color: #fff;
                    z-index: 1000;
                    text-align: center;
                    margin-bottom: 5rem;
                    & span{
                        font-size: inherit;
                        font-family: inherit;
                        color: #00b7ff;
                        z-index: 1000;
                    }
                }

                & p{
                    text-align: center;
                    position: relative;
                    top: 50%;
                    left: 50%;
                    margin-bottom: 5rem;
                    transform: translate(-50%, -50%);
                    color: #fff;
                    font-size: 2vw;
                    font-family: Roboto,sans-serif;
                    font-weight: 600;
                    letter-spacing: 0.1rem;

                }
                #get-started{
                    height: 5rem;
                    width: 15rem;
                    border-radius: 2.5rem;
                    color: rgba(#fff,0.8);
                    border: solid #00b7ff 0.1rem;
                    background-color:rgba(#fff,0);
                    font-family:  Roboto,sans-serif;
                    font-weight: bold;
                    position: relative;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    &:hover{
                        background: #00b7ff;
                    }
                }
            }
        }


    }
</style>