<template>
    <div class="fb_item">
        <div class="fb_data_stars">
            <div class="fb_stars">
                <img src="../assets/images/Modal/Star.svg" alt="">
                <img src="../assets/images/Modal/Star.svg" alt="">
                <img src="../assets/images/Modal/Star.svg" alt="">
                <img src="../assets/images/Modal/Star.svg" alt="">
                <img src="../assets/images/Modal/Star.svg" alt="">
                <img src="../assets/images/Modal/exclamationmark.svg" alt="">
            </div>
            <div class="fb_data">19 января 2023</div>
        </div>
        <div class="fb_item_info">
            <div class="fb_item_info_title">
                Задание «<span>Нужно провести аудит/ проверку сайта</span>»
            </div>
            <div class="fb_item_info_status">Выполнено</div>
            <div class="fb_item_info_client">Заказчик <span>Анастасия Н.</span></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FeedBackItem',
    components: {

    }
}
</script>

<style scoped lang="scss">
.fb_item {
    width: 540px;
    display: flex;
    align-items: baseline;
    padding-bottom: 3rem;
    border-bottom: 1px solid #D9D9D9;
    margin-top: 1rem;

    .fb_item_info{
        font-size: 14px !important;
    }

    .fb_data_stars {
        margin-right: 2rem;
    }

    .fb_item_info_title {
        color: #22305F;
        font-size: 14px;
        font-weight: 700;

        span {
            color: #2D9CDB;
        }
    }

    .fb_item_info_status {
        color: #6FC727;
    }

    .fb_item_info_client {
        color: #828282;
        margin-top: 2rem;

        span {
            color: #2D9CDB;
        }
    }
}

.fb_stars {
    display: flex;
    align-items: center;


    img {
        width: 11px;
        height: 11px;
        margin-right: 0.5rem;
    }
}

.fb_data {
    font-size: 14px;
    color: #828282;
    margin-top: 0.5rem;
}
</style>