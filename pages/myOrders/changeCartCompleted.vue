<template>
    <div class="changeCart">
        <div class="container">
            <OrderNoComplete />
            <div class="changeCart_i">
                <div class="r_side">
                    <div class="o_info">
                        <div class="o_info_i">
                            <div class="order_name">Hire Now дизайн</div>
                            <div class="o_price">до 6 000 руб.</div>
                        </div>
                        <span class="cheks">
                            <img src="../../assets/images/orderCart/eye.svg" alt="eye">
                            <span>112</span>
                        </span>
                    </div>
                    <div class="order_name">Hire Now дизайн</div>
                    <div class="o_price">до 6 000 руб.</div>
                    <span class="stat_order">
                        <span class="time_create" style="color: #EB5757 !important;">
                            Выполнено.
                            <span>Создано 2 февраля 2023 г.</span>
                        </span>
                        <span class="cheks">
                            <img src="../../assets/images/orderCart/eye.svg" alt="eye">
                            <span>112</span>
                        </span>
                        <span class="forward">
                            <img src="../../assets/images/orderCart/hand.svg" alt="">
                            Поделиться заданием
                        </span>
                    </span>
                    <div class="btns_func">
                        <div class="btn_f active">Детали задания</div>
                        <div class="btn_f ">
                            Отклики
                            <div class="count_otclick">5</div>
                        </div>
                    </div>
                    <div class="responses_order" >
                        <div class="warning_order">
                            <img src="../../assets/images/orderCart/warning.svg" alt="">
                            <span class="warning_order_txt">
                                Если вы доверяете исполнителю ценные вещи, крупную задачу<br>
                                или впускаете в дом, проверьте его паспорт и попросите<br>
                                подписать документы. Шаблон расписки, типового договора<br>
                                и другие полезные советы <span>смотрите в рекомендациях.</span>
                            </span>
                        </div>
                        <div class="responses_order_title">
                            Вы можете назначить исполнителем любого пользователя, который оставил<br>
                            отклик к вашему заданию или подождать еще откликов.
                        </div>
                        <div class="rO_filters_btns">
                            <div class="rO_filter_btn active">по рейтингу</div>
                            <div class="rO_filter_btn">по времени</div>
                            <div class="rO_filter_btn">по отзывам</div>
                        </div>
                        <div class="responses_cards">
                            <RespCard />
                            <RespCard />
                            <RespCard />
                        </div>
                    </div>
                    <div class="details_order" >
                        <div class="order_info">
                            <div class="oi_title">
                                Номер задания
                                <div class="">№10666271</div>
                            </div>
                            <div class="oi_title">
                                Категория и подкатегория
                                <div class="">Курьерские услуги - другая посылка</div>
                            </div>
                            <div class="oi_title">
                                Адрес А
                                <div class="">
                                    Красная площадь, Москва
                                </div>
                            </div>
                            <div class="oi_title">
                                Адрес Б
                                <div class="">
                                    улица Арбат, Москва
                                </div>
                            </div>
                            <div class="oi_title">
                                Вернуться в точка А
                                <div class="">
                                    Нет
                                </div>
                            </div>
                            <div class="oi_title">
                                Завершить
                                <div class="">
                                    Среда, 22 февраля 2023 г., 23:59
                                </div>
                            </div>
                            <div class="oi_title">
                                Описание
                                <div class="">
                                    Дизайн сайта и приложения HireNow
                                </div>
                            </div>
                            <div class="oi_title">
                                Приватная информация
                                <div class="">
                                    Не указано
                                </div>
                            </div>
                            <div class="oi_title">
                                Фотография
                                <div class="">
                                    Не указано
                                </div>
                            </div>
                            <div class="oi_title">
                                Предоставить документы
                                <div class="">
                                    Не указано
                                </div>
                            </div>
                        </div>
                        <div class="btn_cancel">Создать еще раз</div>
                        <div class="feedbacks">
                            <div class="feedbacks_title">Отзывы</div>
                            <FeedbackItem />
                        </div>
                    </div>
                </div>
                <div class="side_bar">
                    <div class="all_cat">
                        <div class="all_c_title">Частые вопросы</div>
                        <div class="categ_s">
                            <span>Сколько отликов я получу?</span>
                            <span>Обязательно ли выбирать исполнителя?</span>
                            <span>Какую цену установить?</span>
                            <span>Как оплачивать услуги исполнителя?</span>
                            <span>Как выбрать недежного исполнителя?</span>
                            <span>Как не выбрать исполнителем<br>мошенника?</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import OrderNoComplete from '../../components/Modals/OrderNoComplete.vue';
import FeedbackItem from '../../components/MyOrders/FeedbackItem.vue'
import RespCard from '../../components/MyOrders/RespCard.vue'


export default {
    components: {
        FeedbackItem,
        RespCard,
        OrderNoComplete
    }
}
</script>

<style lang="scss" scoped>
.changeCart {
    padding-top: 4rem;
    padding-bottom: 4rem;
}

.changeCart_i {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 10px;
}

.o_info {
    display: flex;
    justify-content: space-between;
    line-height: normal;
    // align-items: center;
    display: none;

    .o_info_i {
        flex-wrap: wrap;
        gap: 10px;

        .order_name {
            font-size: 22px !important;
        }

        .o_price {
            font-size: 18px !important;
        }
    }

    .cheks {
        img {
            width: 20px;
            height: 13px;
        }

        display: flex;
        height: 13px;
        align-items: center;
        margin-top: 8px;
    }
}

.categ_s {
    color: #2D9CDB;
    font-size: 16px;
    font-weight: 400;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    gap: 25px;
}

.all_c_title {
    font-size: 16px;
    font-weight: 700;
    color: #22305F;
    margin-bottom: 1rem;
}

.r_side {
    width: 700px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.25);
    border-radius: 20px;
    padding: 2rem 4rem;

    .stat_order {
        font-size: 14px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        margin-top: 1rem;
        margin-bottom: 2rem;
    }

    span {
        display: flex;
        color: #828282;

        img {
            margin-right: 0.5rem;
        }
    }

    .time_create {
        color: #6FC727 !important;

        span {
            color: #828282;
            margin-left: 0.4rem;
        }
    }

    .forward {
        color: #2D9CDB;
        cursor: pointer;
    }

    .order_name {
        font-weight: 700;
        font-size: 28px;
        color: #22305F;
    }

    .o_price {
        font-weight: 700;
        font-size: 22px;
        color: #22305F;
    }
}

.btn_f {
    width: 270px;
    height: 40px;
    border: 1px solid #D9D9D9;
    border-radius: 7px 0px 0px 7px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #22305F;
    font-size: 16px;
    font-weight: 400;
    cursor: pointer;

    .count_otclick {
        width: 25px;
        height: 25px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 16px;
        color: white;
        background-color: #FFA200;
        border-radius: 25px;
        margin-left: 0.4rem;
    }
}

.btn_f:last-child {
    width: 270px;
    height: 40px;
    border: 1px solid #D9D9D9;
    border-radius: 0px 7px 7px 0px;
}

.btn_f.active {
    background: #FDEAC2;
}

.btns_func {
    display: flex;
    // justify-content: center;
}

.order_info {
    margin-top: 2rem;

    .grey_block {
        background: #D9D9D9;
        border-radius: 10px;
        width: 100%;
        height: 200px;
        margin-top: 1rem;
    }

    .oi_title {
        font-size: 14px;
        font-weight: 700;
        margin-top: 1rem;
        color: #22305F;

        div {
            font-size: 16px;
            font-weight: 400;
            display: flex;

            img {
                margin-left: .3rem;
                cursor: pointer;
            }
        }
    }
}

.btn_cancel {
    width: 540px;
    height: 50px;
    background: #FFA200;
    border-radius: 60px;
    margin-top: 3rem;
    margin-bottom: 2rem;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 700;
    font-size: 16px;
    color: #FFF;
    cursor: pointer;
    // margin-right: auto;
    // margin-left: auto;
}


.warning_order {
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 115px;
    background: rgba(253, 234, 194, 0.5);
    border-radius: 5px;
    margin-top: 2rem;
    margin-bottom: 2rem;
    padding: 1rem;

    .warning_order_txt {
        display: block;
        font-size: 15px;
        font-weight: 400;
        color: #22305F;

        span {
            display: inline;
            color: #2D9CDB;
            cursor: pointer;
        }
    }
}

.responses_order_title {
    font-size: 15px;
    font-weight: 400;
    color: #828282;
    margin-bottom: 2rem;
}

.rO_filters_btns {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    transition: all .3s;

    .rO_filter_btn {
        width: 130px;
        height: 30px;
        background: #FFFFFF;
        border: 1px solid #828282;
        border-radius: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 15px;
        color: #22305F;
        cursor: pointer;
        transition: all .3s;
    }

    .rO_filter_btn.active {
        background: #FDEAC2;
        border: 1px solid #FDEAC2;
        transition: all .3s;
    }

    .rO_filter_btn:hover {
        background: #FDEAC2;
        border: 1px solid #FDEAC2;
        transition: all .3s;
    }


}

.feedbacks_title {
    font-weight: 700;
    color: #22305F;
    padding-bottom: 2rem;
    margin-top: 5rem;
}

@media (max-width:700px) {

    .rc_btn_choose {
        display: flex;
    }

    .oi_title {
        img {
            display: none;
        }
    }

    .r_side {
        padding: 0 !important;
        width: 95% !important;
        margin-right: auto !important;
        margin-left: auto !important;
        box-shadow: none !important;

        .stat_order {
            flex-wrap: wrap;
            gap: 10px;
        }

        .warning_order_txt {
            font-size: 12px !important;

            br {
                display: none;
            }
        }

        .warning_order {
            height: auto;

            img {
                margin-right: 1rem;
            }
        }

        .rO_filters_btns {
            width: auto;
            flex-wrap: wrap;
            gap: 10px;
        }

        .responses_order_title {
            font-size: 11px;

            br {
                display: none;
            }
        }
    }
}

@media (max-width:580px) {

    .btn_cancel,
    .rc_btn_choose {
        width: 100% !important;
    }
}

@media (max-width:321px) {

    .changeCart {
        padding-top: 5rem;
        padding-bottom: 0rem;
    }

    .o_info {
        display: flex;

        .o_price {
            display: block !important;
        }

        .order_name {
            display: block !important;
        }
    }

    .o_price {
        display: none;
    }

    .order_name {
        display: none;
    }

    .stat_order {
        .cheks {
            display: none;
        }
    }

    .btns_func {
        .btn_f {
            width: 131px;
            height: 26px;
            border: 1px solid #D9D9D9;
            font-size: 12px !important;

            .count_otclick {
                width: 15px;
                height: 15px;
                font-size: 12px !important;
            }
        }
    }

    .oi_title {
        font-size: 12px !important;

        div {
            margin-top: 5px;
            font-size: 12px !important;
        }
    }

    .grey_block {
        height: 125px !important;
    }

    .rc_btn_choose {
        width: 262px !important;
        height: 39px;
        background: #6FC727;
        border-radius: 60px;
        font-size: 12px !important;
        margin-bottom: 0.5rem;
    }

    .btn_cancel {
        width: 262px !important;
        height: 39px;
        font-size: 12px !important;
    }

    .all_c_title {
        font-size: 18px !important;
    }

    .categ_s {
        font-size: 12px !important;
    }

    .warning_order {
        width: 262px;
        height: 143px !important;
        background: rgba(253, 234, 194, 0.5);
        border-radius: 5px;
        padding: 12px;

        .warning_order_txt {
            font-size: 12px !important;
            line-height: 14px !important;
        }

        br {
            display: block !important;
        }
    }

    .rO_filters_btns {
        width: 100%;
        display: flex;
        gap: 15px !important;

        .rO_filter_btn {
            width: 75px;
            height: 24px;
            font-size: 10px;
        }
    }

    .details_order {
        .btn_cancel {
            margin-bottom: 0 !important;
            width: 262px !important;
            height: 39px !important;
            font-size: 12px !important;
            margin-top: 1rem !important;
        }
    }

    .feedbacks_title{
        display: none;
    }
}
</style>
