<template>
    <div data-aos="zoom-in-down"
         data-aos-offset="200"
         data-aos-duration="1000"
         data-aos-easing="ease-in-out"
         data-aos-mirror="true" class="about-us-disc">
        <div class="about-us-disc__inner">
            <h3>Design, Develop &amp; <span>Publish..</span></h3>
            <p>Create an exceptional brand experience across Software Development,
                KelcoTech collaborative environment ensures smarter,
                faster and more efficient Products &amp; Services. Engage with
                Requirements as well as the Customers &amp; route developers to build it.
                Develop the Business with suitable Technologies. Deploy the Business
                over best as well as profitable plateform
            </p>
        </div>
        <div class="about-us-disc__inner">
            <h3>World Class Development
                <span>Tools</span>
            </h3>
            <p>KelcoTech main approach to website design takes into
                account your brand image, your needs and expectations from the site.
                This includes need assessment, planning of content and structure,
                features and functionalities, nomenclature of links, content development,
                designing of theme/homepage and all GUIs. On the whole the complete
                website has to be developed with all the requirements
            </p>
        </div>
        <div class="about-us-disc__inner">
            <h3>
                Analysis &amp;
                <span>Reports</span>
            </h3>
            <p>
                KelcoTech provides a attractive view of your web portal
                with a family of reports. From Twitter &amp; Facebook and other
                networking sites we make you connect specific reports on engagement
                and user performance
            </p>
        </div>
    </div>
    
</template>

<script>
    export default {
        name: "AboutUsDiscriptions"
    }
</script>

<style scoped lang="scss">
    .about-us-disc{
        position: relative;
        display: flex;
        flex-wrap: wrap;
        /*background-color: red;*/
        justify-content: space-around;
        padding: 2rem;
        &__inner{
            width:20vw;
            padding: 5rem;
            margin-right: 5rem;
            display: flex;
            flex-direction: column;
            flex-grow: 1;
            & h3{
                font-size: 1.8rem;
                font-weight: 600;
                letter-spacing: .2rem;
                color: #555;
                text-transform: uppercase;
                font-family: Roboto,sans-serif;
                line-height: 1.6;
                & span{
                    color: #00b7ff;
                }
            }

            & p{
                margin-top: 0.8rem;
                font-size: 1.6rem;
                line-height: 2.2rem;
                color: #606060;
                font-family: Roboto,sans-serif;
                min-width: 25rem;
            }
        }
    }
</style>