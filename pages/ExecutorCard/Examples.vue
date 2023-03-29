<template>
    <div class="exmpls">
        <div class="container">
            <div class="examples">
                <div class="examples_i">
                    <div class="btn_back">
                        <img src="../../assets/images/Arrow.svg" alt="arrow">
                        <span>Вернуться в профиль</span>
                    </div>
                    <div class="e_title">Создание сайтов "Под ключ"</div>
                    <div class="e_sup">В данном фотоальбоме представлены выполненные работы "под ключ"</div>
                    <div class="exapmle_blocks">
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                        <div class="ex_block"></div>
                    </div>
                    <div class="btn_back mobile_no">
                        <img src="../../assets/images/Arrow.svg" alt="arrow">
                        <span>Вернуться в профиль</span>
                    </div>
                    <div class="offer_tsk_btn" >Предложить задание</div>
                </div>
                <div class="side_offer">
                    <div class="offer_job_btn">Предложить задание</div>
                    <div class="offer_job_sup">
                        Исполнитель получит уведомление<br>
                        и сможет оказать вам свои услуги
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import CreatedOfferTask from '../../components/Modals/CreatedOfferTask.vue';
import CreateOfferTask from '../../components/Modals/CreateOfferTask.vue';import Notifications from '../../components/Modals/Notifications.vue';
import OfferTask from '../../components/Modals/OfferTask.vue';



export default {
    components: {
    CreatedOfferTask,
    Notifications,
    CreateOfferTask,
    OfferTask,
    CreateOfferTask
}
}

</script>

<style scoped lang="scss">
.examples {
    padding-top: 2rem;
    padding-bottom: 2rem;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 1rem;

    .e_title {
        font-size: 28px;
        font-weight: 700;
        color: #22305F;
        margin-top: 1rem;
    }

    .e_sup {
        font-size: 16px;
        color: #22305F;
    }

    .btn_back {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        font-size: 14px;
        color: #2D9CDB;
        margin-top: 2rem;
        cursor: pointer;

        span {
            border-bottom: 1px solid #2D9CDB;
            margin-left: .5rem;
            line-height: normal;
        }
    }

    .exapmle_blocks {
        margin-top: 1rem;
        display: flex;
        flex-direction: column;
        gap: 45px;
        align-items: flex-start;
        width: 700px;
        height: 1810px;
        flex-wrap: wrap;

        .ex_block {
            width: 326px;
            height: 326px;
            background-color: #D9D9D9;
            border-radius: 20px;
        }
    }
}

.side_offer {
    padding-top: 4rem;

    .offer_job_btn {
        width: 302px;
        height: 50px;
        background: #6FC727;
        border-radius: 60px;
        justify-content: center;
        align-items: center;
        display: flex;
        color: white;
        margin-right: auto;
        margin-left: auto;
        cursor: pointer;
    }

    .offer_job_sup {
        text-align: center;
        font-size: 16px;
        color: #6FC727;
        margin-top: 5px;
    }
}

@media (max-width:721px) {

    .exapmle_blocks {
        gap: 15px !important;
        width: auto !important;
        height: auto !important;
        align-items: center !important;
    }

    .ex_block {
        width: 240px !important;
        height: 240px !important;
    }
}

@media (max-width:500px) {
    .e_title {
        font-size: 18px !important;
        text-align: center;
    }

    .e_sup {
        font-size: 10px !important;
        text-align: center;
    }
}


@media (max-width:768px) {
    .side_offer{
        display: none !important;
    }

    .btn_back.mobile_no{
        display: none !important;
    }
    .offer_tsk_btn {
        display: flex !important;
        justify-content: center;
        align-items: center;
        width: 230px;
        height: 35px;
        background: #6FC727;
        border-radius: 60px;
        margin-right: auto;
        margin-left: auto;
        margin-top: 2rem;
        color: white;
        font-size: 12px !important;
        font-weight: 700 !important;
        margin-bottom: 2rem;
    }

    .btn_back{
        font-size: 12px !important;
    }

    .e_title{
        font-size: 18px !important;
        text-align: left !important;
    }

    .e_sup{
        font-size: 10px !important;
        text-align: left !important;
    }

}
</style>
