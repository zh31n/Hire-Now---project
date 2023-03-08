<template>
    <div class="modal_messages">
        <div class="modal_messages_i">
            <div class="close_img">
                <img src="../../assets/images/Modal/close.svg" alt="close button" class="close">
            </div>
            <div class="modal_messages_inner">
                <div class="dialogs">
                    <div class="input_d">
                        <input type="text" name="" id="" placeholder="Введите имя для общения">
                    </div>
                    <div class="msg_item">
                        <img src="../../assets/images/Modal/Аватар.svg" alt="">
                        <div class="msg_item_txt">
                            <span class="name">Владислав S.</span><br>
                            <span>Был 01.02.22</span>
                        </div>
                    </div>
                    <div class="msg_item">
                        <img src="../../assets/images/Modal/Аватар.svg" alt="">
                        <div class="msg_item_txt">
                            <span class="name">Владислав S.</span><br>
                            <span>Был 01.02.22</span>
                        </div>
                    </div>
                    <div class="msg_item">
                        <img src="../../assets/images/Modal/Аватар.svg" alt="">
                        <div class="msg_item_txt">
                            <span class="name">Владислав S.</span><br>
                            <span>Был 01.02.22</span>
                        </div>
                    </div>
                    <div class="msg_item">
                        <img src="../../assets/images/Modal/Аватар.svg" alt="">
                        <div class="msg_item_txt">
                            <span class="name">Владислав S.</span><br>
                            <span>Был 01.02.22</span>
                        </div>
                    </div>
                </div>
                <div class="messanger">
                    <div class="messanger_empty">
                        <img src="../../assets/images/Modal/big_msg.svg" alt="">
                        <div class="messanger_empty_title">Выберите, кому хотели бы написать</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ModalMessages',
    components: {

    }
}
</script>

<style scoped lang="scss">
.close_img {
    display: flex;
    justify-content: flex-end;
    width: 96%;
    margin-right: auto;
    margin-left: auto;
    margin-top: 1rem;
    position: relative;
    z-index: 100;

    img {
        cursor: pointer;
    }
}

.modal_messages_inner {
    position: relative;
    bottom: 1.9rem;
    display: flex;
}

.modal_messages {
    position: fixed;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background-color: rgba(0, 0, 0, .3);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;

    .modal_messages_i {
        width: 1100px;
        height: 665px;
        background: #FFFFFF;
        border-radius: 20px;
    }
}

.dialogs {
    width: 350px;
    height: 665px;
    border-right: 1px solid #D9D9D9;
    padding-top: 2rem;

    .input_d {
        width: 315px;
        height: 40px;
        background: #FFFFFF;
        border: 1px solid #D9D9D9;
        border-radius: 5px;
        margin-right: auto;
        margin-left: auto;

        input {
            width: 315px;
            height: 40px;
            border: 0;
            outline: 0;
            padding-left: 1rem;
        }

        input::placeholder {
            color: #828282;
            font-weight: 400;
            font-size: 14px;
        }
    }
}

.msg_item{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    margin-top: 1rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid #D9D9D9;
    img{
        width: 44px;
        height: 44px;
        margin-left: 1rem;
    }

    .msg_item_txt{
        margin-left: 1rem;

        .name{
            font-size: 14px;
            font-weight: 700;
            color: #22305F;
        }

        span{
            font-size: 12px;
            color: #828282;
        }
    }
}

.messanger_empty{
    width: 750px;
    height: 665px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    .messanger_empty_title{
        margin-top: 2rem;
        font-size: 16px;
        font-weight: 700;
        color: #828282;
    }
}
</style>