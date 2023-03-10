<template>
    <div class="response_card">
        <div class="rc_ppl">
            <div class="person_img">
                <img src="../../assets/images/orderCart/person.svg" alt="person">
            </div>
            <div class="person_data">
                <div class="p_name">
                    Сергей С.
                    <img src="../../assets/images/orderCart/veryfied.svg" alt="veryfied">
                </div>
                <div class="p_rating">
                    Рейтинг исполнителя:
                    <img src="../../assets/images/orderCart/Star.svg" alt="starts"> 5.0
                </div>
                <div class="p_count">
                    Нет отзывов - Заказчик
                </div>
            </div>
        </div>
        <div class="rc_info">
            <div class="rc_info_price">Задание «HireNow дизайн» выполнено</div>
            <div class="rc_info_txt">
                Санкт-Петербург! Если понадобится крутой сантехник,<br>
                пишите нам! Мы нашли просто офигенного мужика на<br>
                YouDo, он исправил косяки, которые сделали наши<br>
                прошлые. Мужик простой, но с добрым юмором и очень<br>
                понимающий в своём деле!
            </div>
            <div class="ppl_tel">
                Оценка: 5.0
                <div class="ppl_tel_stars">
                    <img src="../../assets/images/Modal/Star.svg" alt="">
                    <img src="../../assets/images/Modal/Star.svg" alt="">
                    <img src="../../assets/images/Modal/Star.svg" alt="">
                    <img src="../../assets/images/Modal/Star.svg" alt="">
                    <img src="../../assets/images/Modal/Star.svg" alt="">
                </div>
            </div>
            <div class="rc_btns">
                <div class="rc_btn_write">Редактировать отзыв</div>
            </div>
        </div>
        <div class="rc_func">
            <div class="rc_funcs">
                <span class="report">Отзыв виден всем</span>
                <span class="hide">Скрыть</span>
            </div>
            <span class="rc_date">2 февраля</span>
        </div>
    </div>
</template>

<script></script>

<style lang="scss" scoped>
.response_card {
    margin-top: 2rem;
    margin-bottom: 3rem;
}

.rc_ppl {
    display: flex;
    justify-content: flex-start;
    align-items: center;

    .person_data {
        height: 60px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        margin-left: .5rem;

        div {
            display: flex;

            img {
                margin-left: 0.3rem;
                margin-right: 0.3rem;
            }
        }

        .p_name {
            font-weight: 400;
            font-size: 12px;
            color: #2D9CDB;
        }

        .p_rating,
        .p_count {
            font-weight: 400;
            font-size: 12px;
            color: #828282;
        }
    }

    .person_img {
        width: 62px;
        height: 62px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
}

.rc_info {
    width: 540px;
    height: 415px;
    background: #F5F5F5;
    border-radius: 20px;
    margin-top: .5rem;
    padding-top: 2rem;
    padding-left: 2rem;
    padding-right: 2rem;

    .rc_info_price {
        font-size: 16px;
        font-weight: 700;
        color: #22305F;
    }

    .payment_type {
        font-size: 14px;
        font-weight: 700;
        color: #22305F;
        margin-bottom: 2rem;
    }

    .rc_info_txt {
        font-size: 16px;
        color: #22305F;
        margin-bottom: 4rem;
        margin-top: 2rem;
        font-weight: 500 !important;
    }

    .ppl_tel {
        font-weight: 700;
        font-size: 14px;
        color: #22305F;
        display: flex;
        justify-content: flex-start;

        .ppl_tel_stars {
            margin-left: 1rem;
            display: flex;

            img {
                height: 20px;
                width: 20px;
                margin-right: 0.3rem;
            }
        }
    }

    .rc_btns {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .rc_btn_write {
            width: 261px;
            height: 50px;
            background: #FFFFFF;
            border: 2px solid #D9D9D9;
            border-radius: 60px;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-top: 3rem;
            font-weight: 700;
            color: #22305F;
        }
    }
}

.rc_func {
    font-size: 12px;
    font-weight: 400;
    color: #828282;
    display: flex;
    justify-content: space-between;
    width: 95%;
    margin-top: .5rem;

    .rc_funcs {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 30%;
        color: #828282;

        .hide {
            // border-bottom: 1px solid #2D9CDB;
            text-decoration: underline;
            color: #2D9CDB;
            cursor: pointer;
        }

    }
}

@media (max-width:580px) {

    .response_card {
        width: 100%;
        height: auto;
        margin-right: auto;
        margin-left: auto;
    }

    br {
        display: none;
    }

    .rc_info {
        width: 100%;
        height: auto;
        margin-right: auto;
        margin-left: auto;
        padding-top: 1rem;
        padding-left: 1rem;
        padding-right: 1rem;
        padding-bottom: 1rem;
    }

    .rc_btns {
        flex-wrap: wrap;
        gap: 10px;
        margin-top: 1rem;
        margin-bottom: 1rem;

        .rc_btn_write,
        .rc_btn_choose {
            margin: 0 !important;
            width: 100% !important;
            margin-bottom: 1rem;

        }
    }

    .rc_func {
        display: flex;
        justify-content: space-between;

        .rc_funcs {
            display: flex;
            justify-content: flex-start;
            gap: 1rem;
            width: auto;
        }
    }

}
</style>