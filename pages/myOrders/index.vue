<template>
    <div class="myOrders">
        <OrderInProgress />
        <div class="container">
            <div class="myOrders_i">
                <div class="r_side">
                    <PanelInformation />
                    <div class="orderCart">
                        <div class="order_info">
                            <img src="../../assets/images/orderCart/Компьтерная помощь.svg" alt="">
                            <div class="order_info_i">
                                <div class="order_info_title">Установка ПО</div>
                                <div class="order_location">Пушкинская площадь, 5, Москва</div>
                                <div class="o_status">Выполняется</div>
                            </div>
                        </div>
                        <div class="order_price">16 000 ₽</div>
                    </div>
                    <div class="orderCart">
                        <div class="order_info">
                            <img src="../../assets/images/orderCart/Дизайн.svg" alt="">
                            <div class="order_info_i">
                                <div class="order_info_title">Дизайн HireNow</div>
                                <div class="order_location">Можно выполнить удаленно</div>
                                <div class="o_status">Завершить 22 февраля, 23:59</div>
                            </div>
                        </div>
                        <div class="order_price">1 000 ₽</div>
                    </div>
                    <div class="orderCart">
                        <div class="order_info">
                            <img src="../../assets/images/orderCart/Виртуальный помощник.svg" alt="">
                            <div class="order_info_i">
                                <div class="order_info_title">Разработка</div>
                                <div class="order_location">Можно выполнить удаленно</div>
                                <div class="o_status">Отменено</div>
                            </div>
                        </div>
                        <div class="order_price">226 000 ₽</div>
                    </div>
                </div>
                <div class="side_bar">
                    <div class="all_cat">
                        <div class="all_c_title">Все категории</div>
                        <div class="categ_s">
                            <span>Курьерские услуги</span>
                            <span>Ремонт и строительство</span>
                            <span>Грузоперевозки</span>
                            <span>Уборка и помощь по хозяйству</span>
                            <span>Виртуальный помощник</span>
                            <span>Компьютерная помощь</span>
                            <span>Мероприятия и профмоакции</span>
                            <span>Дизайн</span>
                            <span>Разработка ПО</span>
                            <span>Фото, видео и аудио</span>
                            <span>Установка и ремонт техники</span>
                            <span>Красота и здоровье</span>
                            <span>Ремонт цифровой техники</span>
                            <span>Юридическая и бухгалтерская помощь</span>
                            <span>Репетиторы и обучение</span>
                            <span>Ремонт транспорта</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import PanelInformation from '../../components/MyOrders/PanelInformation.vue';
import OrderInProgress from '../../components/Modals/OrderInProgress.vue'

export default {
    components: {
        PanelInformation,
        OrderInProgress
    }
}
</script>

<style lang="scss" scoped>
.myOrders_i {
    display: flex;
    justify-content: space-between;
    width: 95%;
    margin-right: auto;
    margin-left: auto;
    padding-top: 4rem;
    padding-bottom: 4rem;
}

.categ_s {
    color: #2D9CDB;
    font-size: 16px;
    font-weight: 400;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    gap: 25px;
}

.all_c_title {
    font-size: 16px;
    font-weight: 700;
    color: #22305F;
    margin-bottom: 1rem;
}

.orderCart {
    width: 710px;
    height: 180px;
    border: 1px solid #D9D9D9;
    border-radius: 10px;
    padding: 1.5rem 1.5rem;
    display: flex;
    justify-content: space-between;
    margin-top: 1rem;

    .order_price {
        font-weight: 700;
        font-size: 22px;
        color: #22305F;
    }
}

.order_info {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 48%;

    .order_info_i {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 80%;

        .order_info_title {
            font-weight: 700;
            font-size: 22px;
            color: #828282;
        }

        .order_location {
            color: #22305F;
        }

        .o_status {
            font-weight: 700;
            font-size: 14px;
            color: #2D9CDB;
        }
    }

}
</style>