<template>
    <div class="modalChP">
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
                    Не совершайте предоплату без оформления<br>
                    договора или расписки
                </div>
                <div class="modal_warning">
                    <img src="../../assets/images/Modal/warning.svg" alt="">
                    Если доверяете исполнителю ценности или пускаете в дом,<br>
                    зафиксируйте его паспортные данные
                </div>
            </div>
            <div class="modal_btn">Выбрать исполнителя</div>
        </div>
    </div>
</template>

<script>
export default{
    name:'ModalChoosedPerformer',
    components:{

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
    .modalChP_i{
        height: 100vh !important;
        width: 100vw !important;
        border-radius: 0 !important;

        .line{
            width: 50% !important;
        }
    }
}
</style>