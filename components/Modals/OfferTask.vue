<template>
    <div class="modal_task">
        <div class="modal_task_i">
            <div class="close_img">
                <img src="../../assets/images/Modal/close.svg" alt="close button" class="close">
            </div>
            <div class="title">
                Выберите задание, которое<br>
                хотите предложить исполнителю
            </div>
            <div class="select">
                <select name="" id="">
                    <option class="option" value="Новое задание">
                        <img src="../../assets/images/Плюсик.svg" alt="">
                        Новое задание
                    </option>
                    <option class="option" value="Дизайн сайта">Дизайн сайта</option>
                </select>
                <img src="../../assets/images/arr_d.svg" alt="">
            </div>
            <div class="md_sup">
                Каждое задание можно предложить пяти исполнителям<br>
                из каталога. Исполнители получат СМС со ссылкой на ваше<br>
                задание.
            </div>
            <div class="btn">Предложить работу</div>
        </div>
    </div>
</template>

<script >
export default {
    name: 'OfferTask',
    components: {

    }
}
</script>

<style scoped lang="scss">
.modal_task {
    position: fixed;
    height: 100%;
    width: 100%;
    background-color: rgb(0, 0, 0, .3);
    top: 0;
    left: 0;
    display: flex;
    justify-content: center;
    align-items: center;

    .modal_task_i {
        width: 700px;
        height: 563px;
        background: #FFFFFF;
        border-radius: 20px;
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

    .title {
        font-size: 28px !important;
        font-weight: 700;
        color: #22305F;
        text-align: center;
        font-family: inherit;
    }

    .select {
        margin-right: auto;
        margin-left: auto;
        width: 388px;
        height: 40px;
        margin-top: 4rem;
        border: 1px solid #D9D9D9;
        border-radius: 5px;
        overflow: hidden;

        img {
            position: relative;
            bottom: 1.5rem;
            left: 22rem;
            pointer-events: none;
        }

        select {
            width: 100%;
            height: 40px;
            outline: 0;
            padding-left: 1rem;
            padding-right: 1rem;
            color: #828282
        }
    }

    .option{
        color: #22305F;
        border-radius: 10px;
        margin-top: 0.2rem;
    }

    .option:hover{
        background: orange;
        color: white;
    }

    .md_sup {
        font-size: 16px;
        font-weight: 400;
        color: #22305F;
        text-align: center;
        margin-top: 6rem;
    }

    .btn {
        color: white;
        margin-right: auto;
        margin-left: auto;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 240px;
        height: 55px;
        background: #FFA200;
        border-radius: 60px;
        font-size: 16px;
        font-weight: 700;
        margin-top: 6rem;
        cursor: pointer;
    }
}
</style>