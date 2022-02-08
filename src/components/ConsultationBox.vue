<template>
    <div class="container-consultation">
        <div class="container-content">
            
            <h1>
                Start Your Free Consultation
            </h1>

            <p>
                Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium
            </p>

            <button class="button color-gs">
                CONTACT US NOW
            </button>

        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/utility.scss';
@import '@/style/variables.scss';

.container-consultation{
    background: url('/images/CTA-seo-1.jpg') no-repeat center;
    background-size: cover;
    padding:100px 0;
    color:$color-white;
    box-shadow: inset 0px 0px 0 2000px rgba(0,0,0,0.5);

    .container-content{
        width: calc(100%/3);
        margin: 0 auto;
        text-align: center;
        p{
            margin: 30px 0;
        }
    }
}

</style>