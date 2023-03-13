<template>
    <div class="feedback_filters">
        Сначала показывать
        <div class="">
            <div class="fb_btn_filter active">Положительные (163)</div>
            <div class="fb_btn_filter">Отрицательные (0)</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FeedBackButtons',
    components: {

    }
}
</script>

<style scoped lang="scss">
.feedback_filters {
    display: flex;
    align-items: center;
    font-size: 14px;
    color: #828282;
    margin-top: 2rem;
    margin-bottom: 1rem;
    flex-wrap: wrap;
    gap: 10px;

    div {
        display: flex;
        gap: 10px;
        flex-wrap: wrap;
    }
}

.fb_btn_filter {
    width: 150px;
    height: 30px;
    background-color: white;
    border: 1px solid black;
    color: #22305F;
    font-size: 12px;
    font-weight: 500;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 20px;
}

.fb_btn_filter.active {
    background-color: #FDEAC2;
    border: 0;
}

@media (max-width:321px) {
    .feedback_filters {
        align-items: flex-start;
        font-size: 12px !important; 
        .fb_btn_filter {
            width: 117px !important;
            height: 25px !important;
            font-size: 10px !important;
        }

    }
}
</style>