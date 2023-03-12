<template>
    <div v-if="isShow" @click="isShow = false" class="modalChP">
        <div class="modalChP_i">
            <div class="close_img">
                <img src="../../assets/images/Modal/close.svg" alt="close button" class="close">
            </div>
            <div class="modal_title">Оплата напрямую</div>
            <div class="modal_price">
                Стоимость
                <div class="line"></div>
                7 000 ₽
            </div>
            <div class="modal_sup">
                Вы напрямую договариваетесь с исполнителем <br>
                об условиях и способе оплаты.
            </div>
            <div class="modal_warnings">
                <div class="modal_warning">
                    <img src="../../assets/images/Modal/warning.svg" alt="">
                    <span>
                        Не совершайте предоплату без оформления<br>
                        договора или расписки
                    </span>

                </div>
                <div class="modal_warning">
                    <img src="../../assets/images/Modal/warning.svg" alt="">
                    <span>
                        Если доверяете исполнителю ценности или пускаете в дом,<br>
                        зафиксируйте его паспортные данные
                    </span>
                </div>
            </div>
            <div class="modal_btn">Выбрать исполнителя</div>
        </div>
    </div>
</template>

<script>
export default {
    name: "ModalChoosedPerformer",
    data() {
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
        height: 700px;
        width: 700px;
        background-color: white;
        border-radius: 20px;
        text-align: center;
        overflow: auto;

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

        .line {
            width: 380px;
            border: 1px dashed #828282;
            height: 1px;
            margin-top: 20px;
        }

        .modal_title {
            font-size: 28px;
            font-weight: 700;
            color: #22305F;
        }

        .modal_price {
            display: flex;
            justify-content: center;
            margin-top: 5rem;
            font-size: 16px;
            font-weight: 700;
            color: #22305F;
        }

        .modal_sup {
            margin-top: 5rem;
            font-size: 16px;
            font-weight: 700;
            color: #22305F;
            margin-bottom: 5rem;
        }

        .modal_warnings {
            font-size: 14px;
            font-weight: 400;
            color: #22305F;
            text-align: left;
            margin-top: 2rem;

            .modal_warning {
                display: flex;
                justify-content: flex-start;
                align-items: center;
                width: 65%;
                margin-right: auto;
                margin-left: auto;
                margin-top: 2rem;

                img {
                    margin-right: 2rem;
                }
            }
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
        }
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

@media (max-width:321px) {
    .modal_title {
        font-size: 22px !important;
    }

    .modal_price {
        margin-top: 2rem !important;
        font-size: 12px !important;

        .line {
            width: 169px;
            margin-top: 15px !important;
        }
    }

    .modal_sup {
        font-size: 12px !important;
        text-align: center;
        width: 274px;
        margin-right: auto;
        margin-left: auto;
        margin-bottom: 2rem !important;

        br {
            display: none !important;
        }
    }

    .modal_warning {
        font-size: 10px !important;
        width: auto !important;
        gap: 10px !important;

        span {
            width: 210px;
        }

        img {
            margin: 0 !important;
        }

        br {
            display: none;
        }
    }

    .modal_warnings {
        margin-right: auto;
        margin-left: auto;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-top: 0 !important;
    }

    .modal_btn {
        width: 261px !important;
        height: 35px !important;
        background: #6FC727;
        border-radius: 60px;
        font-size: 14px !important;
    }
}
</style>
