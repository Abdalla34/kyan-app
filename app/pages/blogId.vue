<template>
    <div class="blog">
        <PagintaePage class="mt-4 pt-5" />
        <div class="container mt-4">
            <div class="row justify-content-center">
                <div class="col-lg-8 mb-3 col-sm-12">
                    <div class="mini-title mb-4 text-center">
                        <h1 class="title">نشاطات للأطفال 3 سنوات: دليل كيان لدعم ونمو طفلك بشكل سليم!</h1>
                    </div>
                    <div
                        class="d-flex  flex-wrap box-up flex-row-reverse align-items-center justify-content-center gap-2">
                        <div class="box bg-white px-4 py-1 rounded-4">2025 ديسمبر </div>
                        <div class="box bg-white px-4 py-1 rounded-4">5 دقائق للقراءة</div>
                        <div class="box bg-white px-4 py-1 rounded-4"> كيان</div>
                    </div>
                </div>
            </div>
            <div class="row justify-content-center">
                <div class="col-lg-8 col-sm-12">
                    <img class="img rounded-3" src="/blog-3.webp" alt="">
                    <div v-for="item in activities" :key="item.id" class="mb-5 mt-5" dir="rtl">
                        <h2 class="title fs-4 text-end">
                            {{ item.id }}- {{ item.title }}:
                            <span class="fw-normal">{{ item.heading }}</span>
                        </h2>

                        <p class="text-end mt-3">
                            {{ item.description }}
                        </p>

                        <ul class="text-end mt-3">
                            <li v-for="(point, index) in item.points" :key="index">
                                {{ point }}
                            </li>
                        </ul>
                    </div>

                </div>
            </div>
            <div class="row justify-content-center">
                <div class="col-lg-8 col-sm-12">
                    <!-- صناديق المشاركة -->
                    <div class="box-share p-3">

                        <div class="d-flex box-mobile media-content gap-2 flex-wrap justify-content-end mt-3">
                            <button class="telegram d-flex align-items-center gap-1 p-2 rounded-5">
                                #تعليم
                            </button>
                            <button class="whatsapp d-flex align-items-center gap-1 p-2 rounded-5">
                                #تنمية الطفل
                            </button>
                            <button class="twitter d-flex align-items-center gap-1 p-2 rounded-5">
                                #مهارات اجتماعية

                            </button>
                            <button class="facebook d-flex align-items-center gap-1 p-2 rounded-5">
                                #تربية
                            </button>
                            <p>: الوسوم</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row justify-content-center">
                <div class="col-lg-8 box-mobile col-sm-12 text-end rounded-4 p-3 d-flex align-items-center gap-3" style="background-color: rgb(243, 245, 247);">
                    <div>
                        <h3 class="title fs-5">فريق كيان</h3>
                        <p>نحن فريق متخصص في مجال رعاية وتعليم الأطفال، نسعى لمشاركة أحدث المعلومات والنصائح التربوية مع
                            الآباء والأمهات لمساعدتهم في تنشئة أبنائهم بأفضل الطرق.</p>
                    </div>
                    <div class="box-team d-flex align-items-center justify-content-center fs-3 text-white">
                        ف
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
definePageMeta({
    title: "المدونه"
})
const activities = [
    {
        id: 1,
        title: "ركن المسرح",
        heading: "مساحة للتعبير والخيال وبناء الثقة",
        description: `
ركن المسرح من أهم النشاطات المتاحة للأطفال 3 سنوات، لأنه يوفر بيئة تفاعلية تساعد الطفل على التعبير عن نفسه بطريقة طبيعية وسلسة.
    `,
        points: [
            "تطوير مهارات اللغة والنطق",
            "تعزيز الثقة بالنفس",
            "فهم المشاعر والتعبير عنها",
            "تنمية الخيال والإبداع",
            "تقوية المهارات الاجتماعية"
        ]
    },
    {
        id: 2,
        title: "ركن الرسم والفنون",
        heading: "تطوير المهارات الحركية الدقيقة والإبداع",
        description: `
الفنون جزء أساسي من أي برنامج يركز على نشاطات للأطفال 3 سنوات.
    `,
        points: [
            "التلوين بالألوان المائية",
            "القص واللصق",
            "تشكيل الصلصال",
            "صناعة أعمال فنية بسيطة"
        ]
    },
    {
        id: 3,
        title: "النادي الرياضي",
        heading: "تنمية القوة البدنية والمهارات الحركية",
        description: `
الحركة عنصر أساسي في نمو الطفل بعمر 3 سنوات.
    `,
        points: [
            "القفز والجري",
            "ألعاب الكرة الخفيفة",
            "تحسين التوازن",
            "زيادة الثقة بالنفس"
        ]
    },
    {
        id: 4,
        title: "ركن الأنشطة التعليمية",
        heading: "تطوير الذكاء والتفكير المنطقي",
        description: `
تم تصميم هذا الركن ليجمع بين اللعب والمعرفة بدون ضغط.
    `,
        points: [
            "تنمية التفكير المنطقي",
            "تقوية الذاكرة",
            "تعلم الأرقام والألوان",
            "ألعاب البازل والتركيب"
        ]
    },
    {
        id: 5,
        title: "الأنشطة الخارجية",
        heading: "استكشاف الطبيعة والحركة الحرة",
        description: `
أنشطة خارجية داخل مساحات آمنة.
    `,
        points: [
            "اللعب بالرمال",
            "اللعب بالماء",
            "الجري في الهواء الطلق",
            "استكشاف الطبيعة"
        ]
    }
]

</script>
<style scoped>
.box {
    box-shadow: 10px 10px 10px rgb(0, 0, 0, 0.04);
    color: #999696
}



button {
    border: none;
    font-size: 20px;
    padding: 5px 30px !important;
}

button {
    border: none;
    background-color: rgb(243, 245, 247);
    color: #000;
    transition: background-color 0.3s, color 0.3s;
    cursor: pointer;
}


button.facebook:hover {
    background-color: #1877f2;
    /* أزرق فيسبوك */
    color: #fff;
}

button.twitter:hover {
    background-color: #1da1f2;

    color: #fff;
}

button.whatsapp:hover {
    background-color: #25d366;

    color: #fff;
}

button.telegram:hover {
    background-color: #0088cc;

    color: #fff;
}

button.email:hover {
    background-color: #ea4335;

    color: #fff;
}

button.copy-link:hover {
    background-color: #6c757d;

    color: #fff;
}

.box-share {
    margin-bottom: 50px;
    border-top: 1px solid #ccc;
    border-bottom: 1px solid #ccc;
}

.box-team {
    width: 70px;
    height: 60px;    
    background: linear-gradient(to right, #1aaee6, #0d607f);
    border-radius: 50%;
}
@media (max-width: 768px) {
    .title {
        font-size: 16px !important;
    }

    .box-up {
        font-size: 14px !important;
    }
    .box-mobile{
        flex-direction: column-reverse !important;
    }
}
</style>