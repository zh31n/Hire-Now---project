<template>
    <div v-if="isShow" @click="isShow=false" class="response_card">
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
                    Выполнил(-a) 42 задания
                </div>
            </div>
        </div>
        <div class="rc_info">
            <div class="rc_info_price">Стоимость 6000 ₽</div>
            <div class="payment_type">Оплата напрямую</div>
            <div class="rc_info_txt">
                <div style="margin-bottom: 2rem;">Здравствуйте.</div>
                Мой напарник(ца) с достаточным опытом работы, грамотной речью,<br>
                гражданством РФ (РБ) и паспортом готов(а) выполнить Ваше задание.<br>
                Вся ответственность будет лежать на мне. Только, пожалуйста, пишите,<br>
                или лучше звоните, чтобы обсудить детали задания, и уже точно<br>
                доверить его мне и моему сотруднику. Спасибо
            </div>
            <div class="ppl_tel">Телефон исполнителя: <span>+7 999 666-62-22</span></div>
            <div class="rc_btns">
                <div class="rc_btn_write">Написать в чат</div>
                <div class="rc_btn_choose">Выбрать исполнителем</div>
            </div>
            <div class="rc_i_title">
                Выберите исполнителя, чтобы потом оставить отзыв о работе.
            </div>
        </div>
        <div class="rc_func">
            <div class="rc_funcs">
                <span class="report">Пожаловаться</span>
                <span class="hide">Скрыть отклик</span>
            </div>
            <span class="rc_date">2 февраля</span>
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

<style lang="scss" scoped>
.response_card {
    margin-top: 2rem;
    margin-bottom: 3rem;
    width: 540px;
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
    height: 490px;
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
        font-size: 14px;
        color: #22305F;
        margin-bottom: 2rem;
        font-weight: 500 !important;
    }

    .ppl_tel {
        font-weight: 700;
        font-size: 14px;
        color: #22305F;
        display: flex;
        justify-content: flex-start;
        gap: 10px;
        flex-wrap: wrap;
    }

    .rc_btns {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .rc_btn_write,
        .rc_btn_choose {
            width: 220px;
            height: 50px;
            background: #FFFFFF;
            border: 2px solid #D9D9D9;
            border-radius: 60px;
            color: #22305F;
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: 700;
            font-size: 16px;
            cursor: pointer;
            margin-top: 2rem;
            margin-bottom: 2rem;
        }

        .rc_btn_choose {
            background: #6FC727;
            border: 0;
            color: white;
        }
    }

    .rc_i_title {
        font-size: 12px;
        color: #828282;
        font-weight: 400;
    }
}

.rc_func {
    font-size: 12px;
    font-weight: 400;
    color: #828282;
    display: flex;
    justify-content: space-between;
    margin-top: .5rem;

    .rc_funcs {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 33%;

        span {
            border-bottom: 1px solid #828282;
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
