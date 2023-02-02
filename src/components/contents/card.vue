<script>
import btn from './button.vue'

export default {
    name: 'card',
    components: { btn },
    data() {
        return {
            text: 'Get a Consultantion'
        }
    }

}
</script>

<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="img-col">
                    <img src="../../assets/img/card/img1.svg" alt="">
                </div>
                <div class="text-col">
                    <p>Business Growth</p>
                    <h1>Increase Brand Awareness</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt asperiores ut porro in eligendi
                        reiciendis, facilis repudiandae error voluptatem sequi ad!</p>
                    <btn :text="text"></btn>
                </div>
            </div>
        </div>
    </section>
    <section>
        <div class="container">
            <div class="row">
                <div class="text-col">
                    <p>Investors in People</p>
                    <h1>In-House Sales Training</h1>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Illo nemo hic nihil praesentium!
                        Aliquid culpa consectetur esse cum molestiae fugiat reprehenderit atque dolores.</p>
                    <btn :text="text"></btn>
                </div>
                <div class="img-col">
                    <img src="../../assets/img/card/img2.svg" alt="">
                </div>
            </div>
        </div>
    </section>
    <section>
        <div class="container">
            <div class="row">
                <div class="img-col">
                    <img src="../../assets/img/card/img3.svg" alt="">
                </div>
                <div class="text-col">
                    <p>Social Media Analysis</p>
                    <h1>Harness Your Social Proof</h1>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Modi dolores voluptate quas quaerat
                        ipsum adipisci neque ipsam beatae impedit nihil obcaecati iusto, qui quasi.</p>
                    <btn :text="text"></btn>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.container {
    height: 500px;

    margin-top: 5rem;
    margin-bottom: 6rem;

    .row {
        display: flex;
        justify-content: center;
        gap: 3%;
        height: 500px;


        .img-col {
            width: 500px;
        }

        .text-col {

            margin-top: 3rem;
            display: block;
            width: 400px;
            font-size: 1.3rem;

            p {
                font-size: 1.2rem;
                line-height: 2.2rem;
            }
        }

        .text-col>* {
            margin-bottom: 2rem;
        }
    }
}
</style>