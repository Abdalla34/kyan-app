<template>
    <div class="up-header">
        <div class="container p-2">
            <div class="row text-white justify-content-around align-items-center">
                <div class="col-lg-3 d-flex align-items-center gap-3 justify-content-center">
                    <div class="box">
                        <div class="icon"></div>
                        <div class="text">info@futurekayan.com</div>
                    </div>
                    <div class="box">
                        0505996562
                    </div>
                </div>
                <div class="col-lg-6 text-center">
                    الرياض ، حي الرائد ، شارع عبدالعزيز الاحسائي
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
.up-header {
    background-color: var(--main-color);
    border-bottom-left-radius: 40px;
    border-bottom-right-radius: 40px;
    position: relative;
    z-index: 1000;
    width: 70%;
    margin: auto;
    margin-bottom: 40px;
}

@media (max-width:768px) {
    .up-header {
        display: none;
    }
}
</style>