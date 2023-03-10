<template>
    <div class="changeCart">
        <div class="container">
            <div class="changeCart_i">
                <div class="r_side">
                    <div class="order_name">Hire Now дизайн</div>
                    <div class="o_price">до 6 000 руб.</div>
                    <div class="stat_order">
                        <span class="time_create">
                            Открыто.
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
                    </div>
                    <div class="btns_func">
                        <div class="btn_f ">Детали задания</div>
                        <div class="btn_f active">
                            Отклики
                            <div class="count_otclick">5</div>
                        </div>
                    </div>
                    <div class="responses_order">
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
                    <div class="details_order" style="display: none;">
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
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Адрес Б
                                <div class="">
                                    улица Арбат, Москва
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Вернуться в точка А
                                <div class="">
                                    Нет
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="grey_block"></div>
                            <div class="oi_title">
                                Завершить
                                <div class="">
                                    Среда, 22 февраля 2023 г., 23:59
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Описание
                                <div class="">
                                    Дизайн сайта и приложения HireNow
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Приватная информация
                                <div class="">
                                    Не указано
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Фотография
                                <div class="">
                                    Не указано
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Предоставить документы
                                <div class="">
                                    Не указано
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Получить и передать деньги за товар после доставки
                                <div class="">
                                    Не указано
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Какой бюджет?
                                <div class="">
                                    Не указано
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Я используют HireNow для бизнеса и мне нужны закрывающие документы
                                <div class="">
                                    Не указано
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                            <div class="oi_title">
                                Способы оплаты
                                <div class="">
                                    Оплата наличными
                                    <img src="../../assets/images/orderCart/highlighter.svg" alt="">
                                </div>
                            </div>
                        </div>
                        <div class="btn_cancel">Отменить</div>
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
import RespCard from '../../components/MyOrders/RespCard.vue'

export default {
    components: {
        RespCard
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
    gap: 1rem;
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
    background: #FFFFFF;
    border: 2px solid #D9D9D9;
    border-radius: 60px;
    margin-top: 3rem;
    margin-bottom: 2rem;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 700;
    font-size: 16px;
    color: #22305F;
    cursor: pointer;
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
    justify-content: flex-start;
    gap: 1rem;
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

// Media Queries

@media (max-width:700px) {
    .r_side {
        padding: 0 !important;
        width: 95% !important;
        margin-right: auto !important;
        margin-left: auto !important;
        box-shadow: none !important;

        .stat_order{
            flex-wrap: wrap;
            gap: 10px;
        }

        .warning_order_txt{
            font-size: 12px !important;

            br{
                display: none;
            }
        }
        .warning_order{
            height: auto;
            img{
                margin-right: 1rem;
            }
        }

        .rO_filters_btns{
            width: auto;
            flex-wrap: wrap;
            gap: 10px;
        }

        .responses_order_title{
            font-size: 11px;
            br{
                display: none;
            }
        }
    }
}
</style>