<template>
    <div v-if="isShow" @click="isShow = false" class="modal_messages">
        <div class="modal_messages_i">
            <div class="close_img">
                <img src="../../assets/images/Modal/close.svg" alt="close button" class="close">
            </div>
            <div class="modal_messages_inner">
                <MessageDialogs/>
                <div class="messanger" style="display: none;">
                    <div class="messanger_empty">
                        <img src="../../assets/images/Modal/big_msg.svg" alt="">
                        <div class="messanger_empty_title">Выберите, кому хотели бы написать</div>
                    </div>
                    <div class="msg_people">
                        <img src="../../assets/images/Modal/Аватар.svg" alt="">
                        <div class="msg_people_info">
                            <div class="name">Владислав S.</div>
                            <div class="date">Был 01.02.22</div>
                        </div>
                        <img class="muted" src="../../assets/images/Modal/muted.svg" alt="">
                    </div>
                    <div class="msg_messanger">
                        <div class="name_date_guy">
                            <div class="name">Владислав Support Y.</div>
                            <div class="date">02.02.23, 08:04</div>
                        </div>
                        <div class="message_guy">
                            <div>Здравствуйте!</div><br>
                            Ваше задание "75576" удалено.<br>
                            К сожалению, мы не совсем поняли, что все-таки должен сделать<br>
                            исполнитель :( Пожалуйста, уточните вашу задачу и опубликуйте<br>
                            ее вновь.<br><br>
                            Если что, мы всегда рядом - пишите <span>https://youdo.com/supportchat</span> Служба<br>
                            поддержки работает каждый день с 9.00 до 21.00 по<br>
                            московскому времени.
                        </div>
                        <div class="name_date_guy">
                            <div class="name" style="color: #22305F;">Александр</div>
                            <div class="date">4:01</div>
                        </div>
                        <div class="message_guy">
                            Здравствуйте! Ок.
                        </div>
                    </div>
                    <div class="msg_input_send">
                        <img src="../../assets/images/Modal/camera.svg" alt="">
                        <div class="msg_input_send_inp">
                            <input type="text" placeholder="Введите сообщения">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import MessageDialogs from './MessageDialogs.vue';

export default {
    name: "ModalMessages",
    data() {
        return {
            isShow: true,
        };
    },
    components: { MessageDialogs }
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
    // z-index: -10;

    .modal_messages_i {
        width: 1100px;
        height: 665px;
        background: #FFFFFF;
        border-radius: 20px;
    }
}



.messanger_empty {
    width: 750px;
    height: 665px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    .messanger_empty_title {
        margin-top: 2rem;
        font-size: 16px;
        font-weight: 700;
        color: #828282;
    }
}

.messanger {
    width: 750px;
    height: 665px;
}



.msg_messanger {
    height: 490px;
    width: 100%;
    padding-left: 4.5rem;
    overflow: auto;

    .name_date_guy {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 70%;
        margin-top: 2rem;

        .name {
            color: #2D9CDB;
            font-size: 14px;
            font-weight: 700;
        }

        .date {
            color: #828282;
            font-size: 14px;
        }
    }
}

.msg_people {
    height: 80px;
    width: 100%;
    padding-left: 4.5rem;
    padding-top: 1rem;
    display: flex;
    align-items: center;
    justify-content: flex-start;

    .muted {
        margin-left: 1rem;
    }

    .name {
        color: #22305F;
        font-size: 16px;
        font-weight: 700;
    }

    .date {
        color: #828282;
        font-size: 14px;
    }

    img {
        margin-right: 1rem;
    }

}

.msg_input_send {
    height: 92px;
    width: 100%;
    border-top: 1px solid #D9D9D9;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding-left: 2rem;

    img {
        margin-right: 1rem;
    }

    .msg_input_send_inp {
        width: 590px;
        height: 40px;
        border: 1px solid #D9D9D9;
        border-radius: 5px;

        input {
            width: 100%;
            height: 100%;
            outline: 0;
            border: 0;
            padding-left: 1rem;
        }
    }
}

.message_guy {
    margin-top: 2rem;
    font-size: 14px;
    color: #22305F;

    span {
        color: #2D9CDB;
    }
}

@media (max-width: 1161px) {
    .modal_messages_i {
        width: auto !important;
    }

    .msg_input_send_inp {
        width: 80% !important;
    }

}

@media (max-width: 950px) {
    .modal_messages_i {
        width: 700px !important;
        // height: auto !important;

        .msg_people,
        .msg_messanger {
            padding-left: 1rem;
        }
    }


}

@media (max-width: 750px) {
    .input_d {
        width: 250px !important;
    }

    .bl_o {
        margin-left: 20%;
    }

    .trash {
        margin-left: 24% !important;
    }
}

@media (max-width: 750px) {

    .msg_people {
        border-bottom: 1px solid #828282;
        border-top: 1px solid #828282;
    }

    .modal_messages {
        background: none !important;

    }

    .modal_messages_i {
        margin-top: 11% !important;
        // padding-top: 30%;
        width: 100vw !important;
        height: 94.3vh !important;
    }

    .dialogs {
        width: 100%;
        height: 90vh;
        border: none !important;
    }

    .messanger {
        width: 95%;
    }

    .name_date_guy {
        width: 100% !important;
    }
}

@media (max-height: 897px) {
    .msg_messanger {
        height: 75vh;
    }
}

@media (max-height: 750px) {
    .modal_messages_i {
        margin-top: 5rem !important;
    }

    .msg_messanger {
        height: 70vh;
    }
}

@media (max-height: 741px) {
    .msg_messanger {
        height: 70vh !important;
    }
}

@media (max-height: 668px) {
    .msg_messanger {
        height: 65vh !important;
    }
}
@media (max-height: 625px){
    .msg_messanger {
        height: 68vh !important;
    }
}

@media (max-height: 480px) {
    .msg_messanger {
        height: 55vh;
    }
}

@media (max-width: 321px) {
    .close_img {
        display: none;
    }

    .modal_messages .modal_messages_i {
        margin-top: 87px !important;
        border-radius: 0 !important;
    }

    .messanger {
        width: 100% !important;
        padding-top: 2rem !important;

        .msg_people {
            padding-top: 0 !important;
            border-top: 0 !important;
            border-color: #D9D9D9 !important;
        }
        .msg_input_send{
            height: 50px !important;
            border-top: 0 !important;
        }
        .msg_input_send_inp {
            width: 228px !important;
            height: 28px !important;
            font-size: 10px !important;
        }

        .message_guy{
            font-size: 10px !important;
            width: 216px !important;
            margin-top: 1rem !important;

            br{
                display: none !important;
            }
        }

        .name_date_guy{
            width: 95% !important;
            .name{
                font-size: 12px !important;
            }

            .date{
                font-size: 10px !important;
            }
        }
    }
}
</style>
