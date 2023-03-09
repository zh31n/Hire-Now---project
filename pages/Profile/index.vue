<template>
    <div class="profile">
        <div class="container">
            <div class="profile_i">
                <div class="profile_inner">
                    <div class="p_greeting_stat">
                        <div class="p_greeting">Здравствуйте, Антон!</div>
                        <div class="p_views">
                            <img src="../../assets/images/orderCart/eye.svg" alt="">
                            <span>112</span> просмотров профиля
                        </div>
                    </div>
                    <div class="profile_info">
                        <div class="profile_change_img">
                            <div class="profile_img">
                                <img src="../../assets/images/Modal/person.svg" alt="">
                            </div>
                            <div class="change_img_btn">Добавить фото</div>
                        </div>
                        <div class="profile_info_txt">
                            <div class="profile_have_tasks">
                                Создал
                                <span>3 задания</span>
                            </div>
                            <div class="profile_avg_estimate">
                                Средняя оценка 5.0
                                <img src="../../assets/images/Modal/Star.svg" alt="">
                                <span>(2 отзыва)</span>
                            </div>
                        </div>
                    </div>
                    <div class="profile_tab">
                        <div class="about_and_money">
                            <span class="btn_tab ">Обо мне</span>
                            <span class="btn_tab ">Счет</span>
                        </div>
                        <div class="shesternya active">
                            <svg width="23" height="23" viewBox="0 0 23 23" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M10.4267 23H12.5733C13.451 23 14.1384 22.4496 14.3499 21.6029L14.7729 19.7506L15.0478 19.6447L16.6657 20.6503C17.406 21.116 18.2837 20.989 18.9076 20.3645L20.388 18.8827C21.0225 18.2476 21.1283 17.3797 20.663 16.6493L19.6584 15.0299L19.7641 14.7759L21.6147 14.3419C22.4501 14.1302 23 13.4422 23 12.5637V10.4786C23 9.60009 22.4607 8.9121 21.6147 8.70041L19.7747 8.25587L19.669 7.98067L20.6736 6.37184C21.1389 5.64151 21.0331 4.77358 20.3986 4.12793L18.9182 2.64611C18.3048 2.02163 17.4271 1.9052 16.6869 2.36033L15.069 3.35527L14.7729 3.24942L14.3499 1.38656C14.1384 0.539807 13.451 0 12.5733 0H10.4267C9.53839 0 8.85103 0.539807 8.65012 1.38656L8.22713 3.24942L7.93103 3.35527L6.3131 2.36033C5.5623 1.9052 4.69517 2.02163 4.08184 2.64611L2.5908 4.12793C1.9669 4.77358 1.85057 5.64151 2.31586 6.37184L3.32046 7.98067L3.21471 8.25587L1.38529 8.70041C0.53931 8.9121 0 9.60009 0 10.4786V12.5637C0 13.4422 0.549885 14.1302 1.38529 14.3419L3.23586 14.7759L3.33103 15.0299L2.32644 16.6493C1.86115 17.3797 1.97747 18.2476 2.60138 18.8827L4.09241 20.3645C4.70575 20.989 5.58345 21.116 6.32368 20.6503L7.94161 19.6447L8.22713 19.7506L8.65012 21.6029C8.85103 22.4496 9.53839 23 10.4267 23ZM10.7016 21.0525C10.5218 21.0525 10.4267 20.9784 10.4055 20.8196L9.77103 18.2158C9.10483 18.0571 8.45977 17.7819 7.94161 17.4538L5.65747 18.8615C5.52 18.9462 5.3931 18.9356 5.26621 18.8086L4.15586 17.6972C4.02897 17.5808 4.02897 17.4538 4.11356 17.3162L5.52 15.0299C5.22391 14.5219 4.94897 13.8868 4.79034 13.22L2.17839 12.5955C2.01977 12.5743 1.93517 12.4791 1.93517 12.2991V10.7326C1.93517 10.5421 2.0092 10.468 2.17839 10.4257L4.77977 9.81178C4.93839 9.10262 5.24506 8.44639 5.50943 7.97009L4.10299 5.70502C4.01839 5.55683 4.01839 5.42982 4.13471 5.30281L5.25563 4.20202C5.38253 4.0856 5.49885 4.06443 5.65747 4.15969L7.92046 5.54625C8.39632 5.24988 9.10483 4.95352 9.78161 4.78417L10.4055 2.1804C10.4267 2.02163 10.5218 1.93695 10.7016 1.93695H12.2984C12.4782 1.93695 12.5628 2.01104 12.5945 2.1804L13.229 4.79475C13.9163 4.9641 14.5402 5.24988 15.069 5.54625L17.332 4.15969C17.4906 4.07501 17.6069 4.0856 17.7338 4.21261L18.8547 5.31339C18.9816 5.42982 18.9816 5.55683 18.8864 5.70502L17.4906 7.97009C17.7444 8.44639 18.0616 9.10262 18.2202 9.81178L20.8216 10.4257C20.9908 10.468 21.0543 10.5421 21.0543 10.7326V12.2991C21.0543 12.4791 20.9802 12.5743 20.8216 12.5955L18.2097 13.22C18.051 13.8868 17.7655 14.5324 17.4694 15.0299L18.8759 17.3056C18.9605 17.4538 18.9605 17.5702 18.8336 17.6866L17.7232 18.8086C17.5963 18.9356 17.4694 18.9462 17.332 18.8615L15.0584 17.4538C14.5297 17.7819 13.9269 18.0465 13.229 18.2158L12.5945 20.8196C12.5628 20.9784 12.4782 21.0525 12.2984 21.0525H10.7016ZM11.5053 15.5168C13.7048 15.5168 15.5131 13.7069 15.5131 11.4947C15.5131 9.30373 13.7048 7.49379 11.5053 7.49379C9.29517 7.49379 7.47632 9.30373 7.47632 11.4947C7.47632 13.7069 9.29517 15.5168 11.5053 15.5168ZM11.5053 13.6857C10.2998 13.6857 9.31632 12.7013 9.31632 11.4947C9.31632 10.3092 10.3103 9.3249 11.5053 9.3249C12.6791 9.3249 13.6625 10.3092 13.6625 11.4947C13.6625 12.6908 12.6791 13.6857 11.5053 13.6857Z"
                                    fill="#828282" class="orange_h" />
                            </svg>
                        </div>
                    </div>
                    <div class="profile_about_me" style="display: none;">
                        <div class="little_about_me">
                            Немного о себе
                            <div>
                                <img src="../../assets/images/highlighter_grey.svg" alt="">
                                <span>Редактировать</span>
                            </div>
                        </div>
                        <div class="about_exr">
                            Отличный заказчик
                        </div>
                        <div class="block_specifications">
                            <div class="profile_avg_estimate">
                                Средняя оценка 5.0
                                <img src="../../assets/images/Modal/Star.svg" alt="">
                            </div>
                            <div class="block_specifications_i">
                                <div class="spec">
                                    <span>Вежливость</span>
                                    <div class="stars">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                    </div>
                                </div>
                                <div class="spec">
                                    <span>Пунктуальность</span>
                                    <div class="stars">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                    </div>
                                </div>
                                <div class="spec">
                                    <span>Адекватность</span>
                                    <div class="stars">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                        <img src="../../assets/images/Modal/Star.svg" alt="">
                                    </div>
                                </div>
                            </div>
                            <div class="feedback">
                                <div class="title">Отзывы</div>
                                <FeedbackButtons style="margin-bottom: 2rem;" />
                                <FeedBackItem />
                                <FeedBackItem />
                                <FeedBackItem />
                                <FeedBackItem />
                                <FeedBackItem />
                                <FeedBackItem />
                                <FeedBackItem />
                                <FeedBackItem />
                            </div>
                        </div>
                    </div>
                    <div class="profile_score" style="display: none;">
                        <div class="balance">Ваш баланс <span>0</span> ₽</div>
                        <div class="replenish_balance">
                            Пополнить счет на
                            <input class="replBal_inp">
                            ₽
                            <div class="replBal_btn">Пополнить счет</div>
                        </div>
                        <div class="opration_history">
                            <div class="oh_title">История операций</div>
                            <div class="oh_filter">
                                <span class="active">Все операции</span>
                                <span>Пополнения счета</span>
                                <span>Списавния со счета</span>
                            </div>
                            <div class="oh_suop">За данный период транзакций не было</div>
                        </div>
                    </div>
                    <div class="options_tab">
                        <div class="op_btns">
                            <div class="op_btn active">Общие настройки</div>
                            <div class="op_btn">Уведомления</div>
                            <div class="op_btn">Подписка на задания</div>
                            <div class="op_btn">Безопасность</div>
                        </div>
                        <div class="personal_data" style="display: none;">
                            <div class="title">Личные данные</div>
                            <div class="pd_input">
                                <div>Имя</div>
                                <input type="text" name="" id="">
                            </div>
                            <div class="pd_input">
                                <div>Фамилия</div>
                                <input type="text" name="" id="">
                            </div>
                            <div class="pd_sex">
                                <div class="title_sex">Пол</div>
                                <div class="pd_sex_i">
                                    <div class="male">
                                        <div class="oran"></div>
                                        Мужчина
                                    </div>
                                    <div class="male ">
                                        <div class="oran active"></div>
                                        Женщина
                                    </div>
                                </div>
                            </div>
                            <div class="pd_input">
                                <div>Город</div>
                                <input type="text" name="" id="">
                            </div>
                            <div class="pd_input">
                                <div>Email</div>
                                <input type="text" name="" id="">
                            </div>
                            <div class="op_btn_gr">Сохранить личные данные</div>
                        </div>
                        <div class="give_notifiactions" style="display: none;">
                            <div class="title">Получать уведомления:</div>
                            <div class="inps_or">
                                <OrangeInput />
                                Системные уведомления
                            </div>
                            <div class="inps_or">
                                <OrangeInput />
                                Я хочу получать новости сайта
                            </div>
                            <div class="btn">Сохранить</div>
                        </div>
                        <div class="choose_category" style="display: none;">
                            <div class="choose_category_title"></div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Курьерские услуги
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Ремонт и строительство
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Грузоперевозки
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Уборка и помощь по хозяйству
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Виртуальный помощник
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Компьютерная помощь
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Мероприятия и профмоакции
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Дизайн
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Разработка ПО
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Фото, видео и аудио
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Установка и ремонт техники
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Красота и здоровье
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Ремонт цифровой техники
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Юридическая и бухгалтерская помощь
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" alt="">
                                    Репетиторы и обучение
                                </div>
                            </div>
                            <div class="cc_item">
                                <div class="cc_item_title">
                                    <img src="../../assets/images/arr_d.svg" style="transform: rotate(180deg)" alt="">
                                    Ремонт транспорта <span>[3]</span>
                                </div>
                                <div class="cc_btns">
                                    <div class="cc_btn_all_cat">Выбрать все подкатегории</div>
                                    <div class="cc_btns_line">
                                        <div class="cc_btn">Автоэлектрика</div>
                                        <div class="cc_btn active">Шиномонтаж</div>
                                    </div>
                                    <div class="cc_btns_line">
                                        <div class="cc_btn active">Кузовный ремонт</div>
                                        <div class="cc_btn active">Мотосервис</div>
                                        <div class="cc_btn">Что-то другое</div>
                                    </div>
                                </div>
                                <div class="title">Геопозиция. Москва и Новая Москва</div>
                                <div class="pd_input">
                                    <div>Имя</div>
                                    <input type="text" name="" id="">
                                </div>
                                <div class="big_sq"></div>
                                <div class="title">Типы уведомлений</div>
                                <div class="sup">Уведомлять меня по:</div>
                                <div class="or_inps">
                                    <div class="inps_or">
                                        <OrangeInput />
                                        Email
                                    </div>
                                    <div class="inps_or">
                                        <OrangeInput />
                                        Push на телефон
                                    </div>
                                </div>
                                <div class="title">Подборка рекомендованных заданий</div>
                                <div class="sup">
                                    Раз в день мы отправляем на электронный адрес подборку заданий, которые<br>
                                    подходят именно вам.
                                </div>
                                <div class="inps_or" style="width: 100%;margin-bottom: 2rem;">
                                    <OrangeInput />
                                    Получать подборку рекомендованных заданий
                                </div>
                                <div class="btn">Сохранить</div>
                            </div>
                        </div>
                        <div class="security">
                            <div class="title">Изменить пароль</div>
                            <div class="sup">Придумайте новый пароль с такими требованиями:</div>
                            <ul>
                                <li>длина — не менее 8 символов;</li>
                                <li>заглавные буквы;</li>
                                <li>строчные буквы;</li>
                                <li>цифры или специальные символы: %, #, $ и другие.</li>
                            </ul>
                            <div class="pd_input">
                                <div>Новый пароль</div>
                                <input type="text" name="" id="">
                            </div>
                            <div class="pd_input">
                                <div>Повторите пароль</div>
                                <input type="text" name="" id="">
                            </div>
                            <div class="btn">Сохранить</div>
                            <div class="title">Активные сессии</div>
                            <div class="sessions">
                                <img src="../../assets/images/tv.svg" alt="">
                                Текущая — Windows, 2 февраля в 00:00, браузер Opera
                            </div>
                        </div>
                    </div>
                </div>
                <div class="side_bar">
                    <div class="title">Исполнитель</div>
                    <div class="sup">На HireNow с 5 февраля 2023 г.</div>
                    <div class="stat_item">
                        <div class="s_icon" style="background-color: #FFA200;">
                            <img src="../../assets/images/iphone_white.svg" alt="">
                        </div>
                        <div class="s_info">
                            <span class="title">Телефон</span>
                            <span style="color: #22305F;">+7 968 271-88-81</span>
                        </div>
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">Email</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                    <div class="sb_txt">
                        Повысьте доверие пользователей к<br>
                        себе — привяжите ваши аккаунты<br>
                        социальных сетей к профилю<br>
                        HireNow. Мы обязуемся не<br>
                        раскрывать ваши контакты.
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">Tinkoff ID</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">Вконтакте</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">Google</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">mail.ru</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">Однаклассники</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">Apple ID</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                    <div class="stat_item">
                        <div class="s_icon"></div>
                        <div class="s_info">
                            <span class="title">Huawei ID</span>
                            <span>Привязать</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import FeedbackButtons from '../../components/FeedbackButtons.vue';
import FeedBackItem from '../../components/FeedBackItem.vue';
import OrangeInput from '../../components/OrangeInput.vue';

export default {
    components: {
        FeedbackButtons,
        FeedBackItem,
        OrangeInput
    }
}

</script>

<style scoped lang="scss">
.profile {
    padding-top: 2rem;
    padding-bottom: 2rem;

    .profile_i {
        display: flex;
        justify-content: space-between;

        .profile_inner {
            // max-width: 720px;
            width: 720px;

            .p_greeting_stat {
                display: flex;
                justify-content: space-between;
                align-items: center;
            }

        }
    }
}

.p_greeting {
    font-size: 28px;
    font-weight: 700;
    color: #22305F;
}

.p_views {
    display: flex;
    font-size: 14px;
    color: #828282;
    line-height: normal;
    align-items: center;

    span {
        margin-right: 0.5rem;
        margin-left: 0.3rem;
    }

    img {
        margin-right: 0.3rem;
    }
}

.profile_info {
    margin-top: 2rem;
    display: flex;
    align-items: center;

    .change_img_btn {
        width: 184px;
        height: 55px;
        border: 1px solid #D9D9D9;
        border-radius: 60px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 16px;
        color: #22305F;
        font-weight: 700;
        margin-top: 1rem;
    }

    .profile_img {
        width: 183px;
        height: 183px;
        border-radius: 100px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .profile_info_txt {
        margin-left: 3rem;

        .profile_have_tasks {
            font-size: 14px;
            color: #22305F;
            font-weight: 400;
            margin-bottom: 1rem;

            span {
                color: #2D9CDB;
                margin-left: 0.3rem;
            }
        }
    }
}

.profile_avg_estimate {
    display: flex;
    align-items: center;
    padding-bottom: 3rem;
    font-size: 18px;
    color: #22305F;
    font-weight: 700;

    span {
        font-size: 14px;
        font-weight: 500;
        color: #2D9CDB;
        margin-left: 0.3rem;
    }

    img {
        width: 20px;
        height: 20px;
        margin-left: 0.3rem;
    }
}

.profile_tab {
    transition: all .3s;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    border-bottom: 1px solid #D9D9D9;
    padding-bottom: 0.3rem;
    margin-top: 6rem;
    margin-bottom: 3rem;

    .about_and_money {
        font-size: 16px;
        font-weight: 400;
        color: #22305F;

        .btn_tab {
            margin-right: 4rem;
            padding-bottom: 0.4rem;
            cursor: pointer;
        }

        .btn_tab.active {
            border-bottom: 2px solid #FFA200;
            font-weight: 700;
        }
    }

    .shesternya {
        transition: all .3s;
        cursor: pointer;
    }

    .shesternya:hover {
        transition: all .3s;

        .orange_h {
            fill: #FFA200;
        }
    }

    .shesternya.active {
        transition: all .3s;

        .orange_h {
            fill: #FFA200;
        }
    }
}

.little_about_me {
    display: flex;
    align-items: center;
    // margin-top: 2rem;
    font-size: 22px;
    font-weight: 700;
    color: #22305F;

    div {
        cursor: pointer;
        display: flex;
        align-items: center;

        span {
            color: #828282;
            font-size: 12px;
            border-bottom: 1px solid #828282;
        }
    }

    img {
        margin-left: 1rem;
        margin-right: 0.3rem;
    }
}

.about_exr {
    font-size: 14px;
    color: #22305F;
    margin-top: 1rem;
}

.block_specifications {
    background: #FDEAC2;
    border-radius: 10px;
    height: 100px;
    width: 100%;
    padding: 1rem;
    margin-top: 2rem;

    .profile_avg_estimate {
        padding-bottom: 1rem;
    }
}

.spec {
    display: flex;
    align-items: center;

    span {
        margin-right: .5rem;
        font-size: 14px;
        color: #22305F;
    }

    .stars {
        display: flex;

        img {
            margin-right: 0.3rem;
            height: 15px;
            width: 15px;
        }
    }
}

.block_specifications_i {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 95%;
}

.feedback {
    margin-top: 4rem;

    .title {
        font-size: 22px;
        font-weight: 700;
        color: #22305F;
    }
}

.side_bar {
    // max-width: 285px;
    width: 285px;
    border: 1px solid #828282;
    border-radius: 10px;
    height: 700px;
    padding: 0.5rem 1rem;

    .title {
        font-size: 22px;
        color: #22305F;
        font-weight: 700;
    }

    .sup {
        color: #828282;
        font-size: 14px;
    }
}

.stat_item {
    display: flex;
    margin-top: 1rem;
    height: 41px;

    .s_icon {
        width: 41px;
        height: 41px;
        background-color: #D9D9D9;
        border-radius: 5px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .s_info {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        margin-left: 1rem;
        font-size: 14px !important;
        line-height: normal !important;

        .title {
            font-weight: 700;
            color: #22305F;
            line-height: normal !important;
        }

        span {
            font-weight: 400;
            color: #2D9CDB;
            font-size: 14px !important;

        }
    }
}

.sb_txt {
    font-size: 14px;
    font-weight: 400;
    color: #828282;
    margin-top: 1rem;
    margin-bottom: 1rem;
    line-height: 17px;
}

.profile_score {
    .balance {
        font-size: 22px;
        font-weight: 700;
        color: #22305F;
        margin-bottom: 1rem;
    }

    .replenish_balance {
        align-items: center;
        display: flex;
        font-size: 14px;
        color: #22305F;
        margin-top: 1rem;

        .replBal_inp {
            width: 135px;
            height: 45px;
            background: #FFFFFF;
            border: 1px solid #D9D9D9;
            border-radius: 5px;
            outline: 0;
            padding-left: 0.5rem;
            margin-left: 1rem;
            margin-right: 1rem;
        }

        .replBal_btn {
            width: 165px;
            height: 45px;
            background: #6FC727;
            border-radius: 60px;
            color: white;
            font-size: 14px;
            font-weight: 700;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-left: 1rem;
            cursor: pointer;
        }
    }
}

.opration_history {
    width: 640px;
    height: 220px;
    background: #FDEAC2;
    border-radius: 10px;
    padding: 2rem;
    margin-top: 2rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;

    .oh_title {
        font-size: 22px;
        color: #22305F;
        font-weight: 700;
    }

    .oh_filter {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 80%;
        font-size: 14px;
        color: #2D9CDB;
        font-weight: 400;

        span {
            cursor: pointer;
            border-bottom: 1px solid #2D9CDB;
        }

        span.active {
            border: 0;
            color: #22305F;
        }
    }

    .oh_suop {
        font-size: 14px;
        color: #828282;
    }
}

.op_btns {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
    margin-bottom: 2rem;

    .op_btn {
        width: 150px;
        height: 30px;
        border-radius: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 12px;
        color: #22305F;
        background: #FFFFFF;
        border: 1px solid #828282;
        border-radius: 20px;
        cursor: pointer;
    }

    .op_btn.active {
        background: #FDEAC2;
        border: 0;
    }

    .op_btn:hover {
        transition: all .3s;
        background: #FDEAC2;
        border: 0;
    }


}

.personal_data {
    .title {
        font-size: 22px;
        font-weight: 700;
        color: #22305F;
        margin-bottom: 2rem;
    }
}

.pd_input {
    font-size: 14px;
    color: #828282;
    margin-bottom: 1rem;

    div {
        padding-left: 0.5rem;
    }

    input {
        width: 515px;
        height: 40px;
        background: #FFFFFF;
        border: 1px solid #D9D9D9;
        border-radius: 5px;
        padding-left: 1rem;
        outline: 0;
        color: #22305F;
    }
}

.op_btn_gr {
    width: 240px;
    height: 55px;
    background: #6FC727;
    border-radius: 60px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 16px !important;
    // font-weight: 700;
    color: white;
    cursor: pointer;
    margin-top: 4rem;
    line-height: normal;
}

.pd_sex_i {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 50%;
    font-size: 16px;
    color: #22305F;

    .male {
        display: flex;
        align-items: center;

        .oran {
            height: 16px;
            width: 16px;
            border-radius: 10px;
            border: 1px solid black;
            background-color: white;
            margin-right: 1rem;
        }

        .oran.active {
            border: 3px solid #FFA200;
        }
    }
}

.title_sex {
    font-size: 14px;
    color: #828282;
    font-weight: 400;
    margin-bottom: 1rem;
    padding-left: .5rem;
}

.pd_sex {
    margin-bottom: 1rem;
}

.give_notifiactions {
    .title {
        font-size: 22px;
        color: #22305F;
        font-weight: 700;
        margin-bottom: 2rem;
    }



    .btn {
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        font-size: 16px;
        font-weight: 700;
        width: 240px;
        height: 55px;
        background: #6FC727;
        border-radius: 60px;
        margin-top: 2rem;
    }
}

.inps_or {
    display: flex;
    align-items: center;
    width: 40%;
    font-size: 16px;
    margin-bottom: 1rem;
}

.cc_item {
    margin-top: 1rem;
}

.cc_item_title {
    display: flex;
    cursor: pointer;
    align-items: center;

    span {
        color: #FFA200;
        margin-left: 0.5rem;
    }

    img {
        margin-right: 1rem;
    }
}

.cc_btns {

    .cc_btn,
    .cc_btn_all_cat {
        width: 152px;
        height: 30px;
        background: #FFFFFF;
        border: 1px solid #828282;
        border-radius: 20px;
        font-size: 12px;
        color: #22305F;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        line-height: normal;
        margin-right: 1rem;
    }

    .cc_btn_all_cat {
        width: 200px;
        margin-bottom: 1rem;
        margin-top: 1rem;
    }

    .cc_btn.active,
    .cc_btn_all_cat.active {
        background-color: #FDEAC2;
        border: 0;
    }

    .cc_btn:hover,
    .cc_btn_all_cat:hover {
        background-color: #FDEAC2;
        border: 0;
    }
}

.cc_btns_line {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    margin-bottom: 1rem;
}

.cc_item {
    .title {
        font-size: 22px;
        font-weight: 700;
        color: #22305F;
        margin-top: 4rem;
        margin-bottom: 1rem;
    }

    .sup {
        font-size: 14px;
        color: #828282;
        margin-bottom: 2rem;
    }

    .btn {
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        font-size: 16px;
        font-weight: 700;
        width: 240px;
        height: 55px;
        background: #6FC727;
        border-radius: 60px;
        margin-top: 4rem;
    }
}

.big_sq {
    width: 722px;
    height: 228px;
    background: #D9D9D9;
    border-radius: 10px;
    margin-top: 1rem;
    margin-bottom: 1rem;
}

.or_inps {
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #22305F;
    width: 55%;
}

.security {
    .title {
        color: #22305F;
        font-size: 22px;
        font-weight: 700;
        margin-bottom: 2rem;
    }

    .sup {
        font-size: 14px;
        margin-bottom: 1rem;
        color: #22305F;
    }

    ul {
        color: #828282;
        font-size: 12px;
        list-style: disc;
        margin-bottom: 2rem;

        li {
            margin-bottom: 0.5rem;
        }
    }

    .btn {
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        font-size: 16px;
        font-weight: 700;
        width: 240px;
        height: 55px;
        background: #6FC727;
        border-radius: 60px;
        margin-top: 4rem;
        margin-bottom: 3rem;
    }

    .sessions {
        display: flex;
        align-items: center;
        font-size: 14px;

        img {
            margin-right: 0.4rem;
        }
    }
}
</style>