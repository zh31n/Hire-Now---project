<template>
    <div class="modalChP">
        <div class="modalChP_i">
            <div class="close_img">
                <img src="../../assets/images/Modal/close.svg" alt="close button" class="close">
            </div>
            <div class="modalChP_inner">
                <div class="modal_title">Задание не выполнено</div>
                <div class="rating_guy">
                    Пожалуйста, укажите причину, по которой задание не было выполнено:
                </div>
                <div class="choose_vars">
                    <div class="var">
                        <div class="inp_circle active"></div>
                        Случайно выбрал не того исполнителя
                    </div>
                    <div class="var">
                        <div class="inp_circle "></div>
                        Исполнитель изменил условия сотрудничества
                    </div>
                    <div class="var">
                        <div class="inp_circle "></div>
                        Исполнитель отказался выполнять задание
                    </div>
                    <div class="var">
                        <div class="inp_circle "></div>
                        Исполнитель опоздал
                    </div>
                    <div class="var">
                        <div class="inp_circle "></div>
                        Работа выполнена не полностью или некачественно
                    </div>
                    <div class="var">
                        <div class="inp_circle "></div>
                        Я столкнулся с мошенничеством
                    </div>
                    <div class="var">
                        <div class="inp_circle "></div>
                        Задание перестало быть актуальным
                    </div>
                    <div class="var">
                        <div class="inp_circle "></div>
                        Другая причина
                    </div>
                </div>
            </div>
            <div class="modal_btn">Продолжить</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'OrderNoComplete'
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
        // text-align: center !important;
        background-color: white;
        border-radius: 20px;
        overflow-y: auto;
        overflow-x: hidden;

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
            font-size: 16px;
            font-weight: 400;
            color: #22305F;
            text-align: left;
            margin-top: 2rem;
            padding-bottom: 2rem;
        }

        .modal_title {
            font-size: 28px;
            font-weight: 700;
            color: #22305F;
            margin-left: auto;
            margin-right: auto;
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
}

.choose_vars {
    margin-top: 2rem;
}

.var {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    margin-top: 1rem;
    color: #22305F;
    font-size: 16px;

    .inp_circle {
        width: 16px !important;
        height: 16px !important;
        border-radius: 50px;
        border: 1px solid grey;
        margin-right: 1rem;
    }

    .inp_circle.active {
        border: 3px solid #FFA200;
    }
}


@media (max-height:700px) {
    .modalChP_i {
        height: 100vh !important;
        width: 100vw !important;
        border-radius: 0 !important;

        .line {
            width: 50% !important;
        }
    }
}

@media (max-width:540px) {
    .modal_title {
        font-size: 22px !important;
    }

    .rating_guy {
        display: none;
    }

    .choose_vars {


        .var {
            font-size: 12px !important;
            margin-left: 5rem;
        }

        .inp_circle {
            margin-right: 0.5rem !important;
        }
    }


}

@media (max-width:400px) {
    .var {
        font-size: 12px !important;
        margin-left: 0rem !important;
    }

    .modal_title {
        padding-left: 2rem;
    }

}
</style>