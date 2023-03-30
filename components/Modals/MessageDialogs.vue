<template>
    <div class="dialogs">
        <div class="input_d">
            <input type="text" name="" id="" placeholder="Введите имя для общения">
        </div>
        <div class="close_img" style="display: none;" v-if="isShow" @click="isShow = false">
            <img src="../../assets/images/Modal/close.svg" alt="close button" class="close">
        </div>
        <div class="msg_items">
            <div class="msg_item active">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
            </div>
            <div class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
            </div>
            <div class="msg_item ">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
            </div>
            <div class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name" style="color: orange;">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
                <div class="bl_o">2</div>
            </div>
            <div class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name" style="color: orange;">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
                <div class="bl_o">2</div>
            </div>
            <div class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name" style="color: orange;">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
                <div class="bl_o">2</div>
            </div>
        </div>
        <div class="msg_items mobile">
            <NuxtLink to="/Messages/1" class="msg_item active">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
            </NuxtLink>
            <NuxtLink to="/Messages/1" class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
            </NuxtLink>
            <NuxtLink to="/Messages/1" class="msg_item ">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
            </NuxtLink>
            <NuxtLink to="/Messages/1" class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name" style="color: orange;">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
                <div class="bl_o">2</div>
            </NuxtLink>
            <NuxtLink to="/Messages/1" class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name" style="color: orange;">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
                <div class="bl_o">2</div>
            </NuxtLink>
            <NuxtLink to="/Messages/1" class="msg_item">
                <img src="../../assets/images/Modal/Аватар.svg" alt="">
                <div class="msg_item_txt">
                    <span class="name" style="color: orange;">Владислав S.</span><br>
                    <span>Был 01.02.22</span>
                </div>
                <img class="trash" src="../../assets/images/Modal/trash.svg" alt="">
                <div class="bl_o">2</div>
            </NuxtLink>
        </div>
    </div>
</template>
<script>
export default {
    name: 'MessageDialogs',
    data() {
        return {
            isShow: true,
        }
    }
}
</script>

<style scoped lang="scss">
.msg_items.mobile {
    display: none;
}

.dialogs {
    width: 350px;
    height: 665px;
    border-right: 1px solid #D9D9D9;
    padding-top: 2rem;
    transition: all .3s;

    .input_d {
        width: 315px;
        height: 40px;
        background: #FFFFFF;
        border: 1px solid #D9D9D9;
        border-radius: 5px;
        margin-right: auto;
        margin-left: auto;
        margin-bottom: 1rem;

        input {
            width: 100%;
            height: 100%;
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

.bl_o {
    margin-left: 40%;
    background-color: orange;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50px;
    color: white;
    width: 30px;
    height: 30px;
    font-size: 16px;
    font-weight: 700;
}

.msg_item.active {
    background-color: #D9D9D9;

    .trash {
        margin-left: 40%;
        display: block;
        cursor: pointer;
    }
}

.msg_item:hover {
    // background-color: #D9D9D9;
    transition: all .3s;

    .trash {
        margin-left: 40%;
        display: block;
    }

    .bl_o {
        display: none;
    }
}

.msg_item {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding-top: 1rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid #D9D9D9;
    // cursor: pointer;
    transition: all .3s;
    position: relative;
    z-index: 100;

    img {
        margin-left: 1rem;
    }

    .trash {
        margin-left: 40%;
        display: none;
    }

    .msg_item_txt {
        margin-left: 1rem;

        .name {
            font-size: 14px;
            font-weight: 700;
            color: #22305F;
        }

        span {
            font-size: 12px;
            color: #828282;
        }
    }
}

@media (max-width:768px) {
    .msg_items {
        height: 70vh !important;
        overflow: auto;
    }

    .close_img {
        display: block !important;
        padding-left: 30px;
        margin-bottom: 1rem;
    }

    .bl_o,
    .trash {
        margin-left: 23% !important;
    }

    .input_d {
        width: 261px !important;
        height: 30px !important;
        margin-right: auto;
        margin-left: auto;
        margin-top: 2rem;
    }

    .input_d input::placeholder {
        font-size: 10px !important;
    }

    .input_d input {
        padding-bottom: 5px;
    }

    .msg_item {
        width: 261px !important;
        margin-right: auto;
        margin-left: auto;
    }
    .msg_items{
        display: none;
    }

    .msg_items.mobile {
        display: block;
    }
}
</style>
