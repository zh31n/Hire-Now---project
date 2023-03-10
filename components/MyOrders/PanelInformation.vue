<template>
    <div class="panel_info">
        <div class="btns_func">
            <div class="btn_f">Я исполнитель</div>
            <div class="btn_f active">Я заказчик</div>
        </div>
        <div class="info">
            <span>Всего вы создали <span>3</span> задания(-ий) , из них:</span>
            <div class="info_orders">
                <span class='i_orders_item'>Открыто: <span>66</span></span>
                <span class='i_orders_item'>Выполняется: <span>2</span></span>
                <span class='i_orders_item'>Выполнено: <span>243</span></span>
            </div>
        </div>
        <div class="point_buis">
            <div class="elipse">
                <div class="elipse"></div>
            </div>
            <span>Бизнес-задания</span>
        </div>
    </div>
</template>

<script>

</script>

<style scoped lang="scss">
.panel_info {
    width: 710px;
    height: 290px;
    box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.25);
    border-radius: 10px;
    padding-top: 2rem;
    margin-bottom: 2rem;
}

.btn_f {
    width: 270px;
    height: 40px;
    border: 1px solid #D9D9D9;
    border-radius: 7px 0px 0px 7px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #22305F;
    font-size: 16px;
    font-weight: 400;
}

.btn_f:last-child {
    width: 270px;
    height: 40px;
    border: 1px solid #D9D9D9;
    border-radius: 0px 7px 7px 0px;
}

.btn_f.active {
    background: #FDEAC2;
}

.btns_func {
    display: flex;
    margin-left: 2rem;
}

.info {
    font-weight: 700;
    color: #22305F;
    font-size: 16px;
    background: 0 !important;
    border: 0 !important;
    margin-left: 2rem;
    margin-top: 3rem;
}

.info_orders {
    margin-top: 2rem;
    display: flex;
    justify-content: space-between;
    width: 60%;
}

.i_orders_item {
    span {
        color: #2D9CDB;
        margin-left: .2rem;
    }
}

.point_buis {
    margin-left: 2rem;
    margin-top: 2rem;
    display: flex;
    align-items: center;

    span {
        font-weight: 400;
        font-size: 16px;
        color: #22305F;
        margin-left: 1rem;
    }
}

.elipse {
    width: 16px;
    height: 16px;
    border-radius: 50px;
    background-color: orange;
    display: flex;
    justify-content: center;
    align-items: center;

    .elipse {
        background-color: white;
        width: 10px;
        height: 10px;
    }
}

@media (max-width: 768px) {

    .panel_info {
        text-align: center;
        width: auto;
        min-width: 560px;
        box-shadow: none;
    }

    .btns_func {
        width: 100%;
        justify-content: center;
        margin-left: 0;
    }

    .info_orders {
        justify-content: center;
        gap: 2rem;
        width: 100%;
    }

    .info {
        margin-left: 0;
    }

    .point_buis {
        justify-content: center;
        margin-left: 0;
    }
}

@media (max-width: 580px) {
    .btn_f {
        width: 200px !important;
    }

    .panel_info {
        min-width: 460px !important;
    }
}


@media (max-width: 480px) {
    .btn_f {
       min-width: 120px !important;
       width: auto !important;
       font-size: 12px;
    }

    .panel_info {
        min-width: 300px !important;
    }

    .info {
        margin-top: 1rem;

        .info_orders {
            gap: 4px;
            flex-direction: column;
            margin-top: 10px;
        }
    }
}

</style>