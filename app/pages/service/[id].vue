<template>
    <div class="single-serv mt-5 pt-5">
        <PagintaePage />
        <div class="container mt-4 mb-5">
            <div class="parent" v-if="singleServ"></div>
            <div class="row justify-content-center align-items-center">
                <div class="col-lg-5 text-end col-md-6 col-sm-12">
                    <div class="mini-title-sec mb-4 text-end">
                        <h5> أركان المركز</h5>
                        <h1 class="title ">
                            {{ singleServ.title }}
                        </h1>
                        <p class="mt-4">{{ singleServ.desc }}</p>

                        <div>
                            <Btn text="احجزي لطفلك الآن" />
                        </div>
                    </div>

                </div>
                <div class="col-lg-3 col-md-6 col-sm-12">
                    <div class="img-circle" :class="singleServ.color">
                        <img :src="singleServ.image" alt="">
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-color-section">
            <WaveUp />
            <div class="container p-5 text-center">
                <div class="row justify-content-center">
                    <div class="col-lg-8 col-md-8 col-sm-12">
                        <div class="mini-title-sec mb-4 text-center">
                            <h5> تعلم اللغات في كيان</h5>
                            <h1 class="title ">
                                جسر يربط الأطفال <span class="span-title">بثقافات العالم</span>
                            </h1>
                            <p class="mt-4">في عالمٍ يتسم بالتنوع والتواصل المستمر، يعتبر تعلم اللغات جسرًا حيويًا يربط
                                الأطفال
                                بثقافات العالم المختلفة. يسهم إتقان لغة جديدة في توسيع آفاق الطفل، وتعزيز فهمه واحترامه
                                للتنوع
                                الثقافي، وسنكتشف سويًا كيف يمكن لتعلم اللغات أن يكون تجربة ممتعة وفعالة للأطفال، مع
                                التركيز على
                                الأساليب التفاعلية والفوائد المتعددة لبدء هذه الرحلة في سن مبكرة.

                            </p>

                            <div class="mt-4">
                                <Btn text="احجزي لطفلك الآن" />
                            </div>
                        </div>
                    </div>
                </div>

            </div>
            <div class="wave-rotate">
                <WaveDown />
            </div>
        </div>
        <!-- Section imge learn -->
        <div class="container mt-5 text-center">
            <div class="row justify-content-between align-items-center">
                <!-- img -->
                <div class="col-lg-3 col-md-6 col-sm-12">
                    <div class="img-circle">
                        <img :src="singleServ.image" alt="">
                    </div>
                </div>
                <!-- text -->
                <div class="col-lg-8 text-end col-md-6 col-sm-12">
                    <div class="mini-title-sec mb-4 text-end">
                        <h5>تعلم بمتعة</h5>
                        <h1 class="title">
                            تعلم اللغات للأطفال <span class="span-title">بسهولة ومتعة</span>
                        </h1>
                        <p class="mt-4">
                            يعد تقديم اللغات للأطفال بطريقة مرحة وتفاعلية أمرًا أساسيًا لجعل عملية التعلم ممتعة وفعّالة.
                            الأساليب التقليدية قد تكون مملة أو معقدة للأطفال، لذا من الأفضل استخدام تقنيات تدمج بين
                            التعلم واللعب.
                        </p>
                        <p class="mt-4">
                            على سبيل المثال، يمكن استخدام الألعاب التفاعلية، الأغاني، والقصص المصورة لتقديم المفردات
                            والتراكيب اللغوية بطريقة جذابة. تظهر الدراسات أن الأطفال يتعلمون بشكل أفضل عندما يكونون
                            مستمتعين ومشاركين بنشاط في العملية التعليمية.
                        </p>
                    </div>
                </div>
            </div>
        </div>
        <!-- contact -->
        <contact />

    </div>
</template>
<script setup>
import WaveDown from '~/components/icons/waveDown.vue'
import WaveUp from '~/components/icons/waveUp.vue'

definePageMeta({
    title: "أركانرالمركز"
})
const { services } = useServices()
const route = useRoute()

const id = Number(route.params.id)

const singleServ = computed(() => {
    return services.find(serv => serv.id === id)
})
</script>