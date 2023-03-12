<template>
    <div v-if="isShow" @click="isShow=false" class="notifications">
        <div class="title">Уведомления</div>
        <div class="otklick_items">
            <div class="otklick_item">
                <div class="otklick_item_date">вчера 13:11</div>
                <div class="otklick_item_info">
                    <img src="../../assets/images/applepencil.svg" alt="">
                    <div class="otklick_item_txt">
                        <div class="title">
                            1 Новый отклик <span>к заданию</span>
                        </div>
                        <div class="sup">«Доставить один пакет»</div>
                    </div>
                </div>
            </div>
            <div class="otklick_item">
                <div class="otklick_item_date">вчера 13:11</div>
                <div class="otklick_item_info">
                    <img src="../../assets/images/applepencil.svg" alt="">
                    <div class="otklick_item_txt">
                        <div class="title">
                            1 Новый отклик <span>к заданию</span>
                        </div>
                        <div class="sup">«Доставить один пакет»</div>
                    </div>
                </div>
            </div>
            <div class="otklick_item">
                <div class="otklick_item_date">вчера 13:11</div>
                <div class="otklick_item_info">
                    <img src="../../assets/images/applepencil.svg" alt="">
                    <div class="otklick_item_txt">
                        <div class="title">
                            1 Новый отклик <span>к заданию</span>
                        </div>
                        <div class="sup">«Доставить один пакет»</div>
                    </div>
                </div>
            </div>
            <div class="otklick_item">
                <div class="otklick_item_date">1 день назад</div>
                <div class="otklick_item_info">
                    <img src="../../assets/images/applepencil.svg" style="opacity: 0;" alt="">
                    <div class="otklick_item_txt">
                        <div class="title">
                            1 Новый отклик <span>к заданию</span>
                        </div>
                        <div class="sup">«Доставить один пакет»</div>
                    </div>
                </div>
            </div>
            <div class="otklick_item">
                <div class="otklick_item_date">1 день назад</div>
                <div class="otklick_item_info">
                    <img src="../../assets/images/applepencil.svg" style="opacity: 0;" alt="">
                    <div class="otklick_item_txt">
                        <div class="title">
                            1 Новый отклик <span>к заданию</span>
                        </div>
                        <div class="sup">«Доставить один пакет»</div>
                    </div>
                </div>
            </div>
        </div>
        <div class="type_btns">
            <span>Отметить все как<br>прочитанные</span>
            <span>Показать еще</span>
        </div>
    </div>
</template>

<script>
export default {
  data(){
    return {
      isShow: true,
    }
  }
}
</script>

<style scoped lang="scss">
.notifications {
    width: 340px;
    height: 477px;
    background: #FFFFFF;
    box-shadow: 0px 6px 10px 0px rgba(0, 0, 0, 0.25);
    border-radius: 5px;
    border-top-left-radius: 0;
    border-top-right-radius: 0;
    position: absolute;
    top:100%;
    right: 10%;
    z-index: 1;

    .title {
        font-size: 16px;
        font-weight: 700;
        color: #22305F;
        margin-left: 1rem;
        margin-top: .5rem;
    }

    .otklick_item_date {
        font-size: 10px;
        color: grey;
        text-align: right;
        margin-right: 0.3rem;
    }

    .otklick_item_info {
        display: flex;
        padding-left: 1rem;

    }

    .otklick_item {
        padding-bottom: 1rem;
        border-bottom: 1px solid #828282;
    }

    .otklick_item_txt {
        margin-left: 1rem;

        .title {
            font-size: 14px !important;
            font-weight: 700;
            color: #22305F;
            margin: 0;
            line-height: normal;

            span{
                font-weight: 400 !important;
            }
        }

        .sup {
            font-size: 14px;
            font-weight: 400;
            color: #828282;
            text-decoration: underline;
            // line-height: 120%;
        }
    }
}

.type_btns{
    width: 90%;
    margin-right: auto;
    margin-left: auto;
    display: flex;
    justify-content: space-between;
    color: #6FC727;
    font-size: 12px;
    align-items: center;
    margin-top: 1.5rem;

    span{
        cursor: pointer;
    }
}

@media (max-width:381px) {
    .notifications{
        right: 0;
        width: 100%;
    }

}
</style>
