<template>
    <div v-if="isShow" @click="isShow=false" class="modalChP">
        <div class="modalChP_i">
            <div class="close_img">
                <img src="../../assets/images/Modal/close.svg" alt="close button" class="close">
            </div>
            <div class="modalChP_inner">
                <div class="modal_title">Задание выполнено</div>
                <div class="rating_guy">Оцените исполнителя</div>
                <div class="estimations_guy">
                    <div class="estimation_line">
                        Качество
                        <div class="est_stars">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                        </div>
                    </div>
                    <div class="estimation_line">
                        Вежливость
                        <div class="est_stars">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star.svg" alt="">
                            <img src="../../assets/images/Modal/Star_empty.svg" alt="">
                        </div>
                    </div>
                    <div class="estimation_line">
                        Стоимость услуг
                        <div class="est_stars">
                            <img src="../../assets/images/Modal/Star_empty.svg" alt="">
                            <img src="../../assets/images/Modal/Star_empty.svg" alt="">
                            <img src="../../assets/images/Modal/Star_empty.svg" alt="">
                            <img src="../../assets/images/Modal/Star_empty.svg" alt="">
                            <img src="../../assets/images/Modal/Star_empty.svg" alt="">
                        </div>
                    </div>
                </div>
                <div class="feedback_block">
                    <div class="fbk_title">Отзыв</div>
                    <div class="fbk_sup">
                        Этот отзыв будет опубликован в профиле исполнителя и поможет<br>
                        другим заказчикам принять верное решение.
                    </div>
                    <textarea class="input_fbk"></textarea>
                    <div class="input_hint">Отзыв должен содержать от 10 до 4000 символов.</div>
                </div>
                <div class="info_yo">
                    <div class="info_yo_title">Информация для YouDo</div>
                    <div class="info_yo_sup">
                        Эта информация не будет опубликована на странице исполнителя,<br>
                        её увидят только модераторы YouDo.
                    </div>
                    <div class="choose_vars">
                        <div class="var">
                            <div class="inp_circle active"></div>
                            Я не рекомендую этого исполнителя
                        </div>
                        <div class="var">
                            <div class="inp_circle "></div>
                            Задание выполнял другой исполнитель без согласования со мной
                        </div>
                    </div>
                </div>
                <div class="modal_btn">Оставить отзыв</div>
            </div>
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
.modalChP {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, .5);
    z-index: 2000;
    transition: .3s all;
    display: flex;
    justify-content: center;
    align-items: center;

    .modalChP_i {
        width: 700px;
        height: 700px;
        background-color: white;
        border-radius: 20px;
        overflow: auto;

        .modalChP_inner {
            width: 525px;
            margin-right: auto;
            margin-left: auto;

            .estimations_guy {
                margin-top: 4rem;
            }

            .estimation_line {
                display: flex;
                justify-content: space-between;
                align-items: center;
                margin-bottom: 2rem;
                font-weight: 400;
                font-size: 22px;
                color: #22305F;
            }

            .est_stars {
                display: flex;
                justify-content: space-between;
                width: 240px;
            }
        }

        .close_img {
            display: flex;
            justify-content: flex-end;
            width: 96%;
            margin-right: auto;
            margin-left: auto;
            margin-top: 1rem;

            img {
                cursor: pointer;
            }
        }

        .rating_guy {
            font-size: 18px;
            font-weight: 700;
            color: #22305F;
            text-align: left;
            margin-top: 4rem;
        }

        .modal_title {
            font-size: 28px;
            font-weight: 700;
            color: #22305F;
            text-align: center;
        }

        .modal_btn {
            width: 240px;
            height: 55px;
            background: #6FC727;
            border-radius: 60px;
            font-weight: 700;
            font-size: 16px;
            color: #FFFFFF;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-right: auto;
            margin-left: auto;
            margin-top: 6rem;
            margin-bottom: 2rem;
        }
    }

}

.feedback_block {
    margin-top: 4rem;

    .fbk_title {
        font-size: 18px;
        font-weight: 700;
        color: #22305F;
    }

    .fbk_sup {
        font-size: 14px;
        color: #22305F;
        margin-top: 1rem;
    }

    .input_fbk {
        width: 100%;
        height: 200px;
        border: 1px solid #828282;
        border-radius: 10px;
        resize: none;
        outline: 0;
        padding: .5rem;
        margin-top: 1rem;
    }

    .input_hint {
        margin-top: 1rem;
        color: #828282;
        font-size: 14px;
    }
}

.info_yo {
    margin-top: 2rem;

    .info_yo_title {
        font-size: 18px;
        font-weight: 700;
        color: #22305F;
        margin-bottom: 1rem;
    }

    .info_yo_sup {
        font-size: 15px;
        font-weight: 400;
        color: #22305F;
    }

    .choose_vars{
        margin-top: 2rem;
    }

    .var{
        display: flex;
        justify-content: flex-start;
        align-items: center;
        margin-top: 1rem;
        color: #22305F;
        font-size: 16px;

        .inp_circle{
            width: 16px;
            height: 16px;
            border-radius: 50px;
            border: 1px solid grey;
            margin-right: 1rem;
        }

        .inp_circle.active{
            border: 3px solid #FFA200;
        }
    }
}
</style>
