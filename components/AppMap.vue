<template>
    <div class="map__content">
        <div class="map__content_left">
            <div class="map__title">
                Выберите ПВЗ
            </div>
            <div class="map__sup">Выберите пункт доставки</div>
            <ul class="map__list">
                
                <li v-for="coord in coords" class="map__item">
                    <div class="map_list_cont">
                        {{ coord?.officeAddress }}
                        <div class="time__map">
                            Ежедневно<br>
                            10:00-21:00
                        </div>
                    </div>
                </li>
                
            </ul>
        </div>
        <div class="map ui-map" ref="map"></div>
    </div>
</template>

<script>
import ymaps from 'ymaps';

export default {
    mounted() {
        ymaps
            .load('https://api-maps.yandex.ru/2.1/?lang=ru_RU')
            .then(maps => {
                const myMap = new maps.Map(this.$refs.map, {
                    center: [45.038605, 41.905666],
                    zoom: 7
                });


                this.coords.forEach(coord => {
                    const placemark = new maps.Placemark([coord?.OfficeLatitude, coord?.OfficeLongitude], {
                        hintContent: coord?.officeAddress,
                        balloonContent: coord?.officeAddress
                    }, {
                        // iconLayout: 'default#image',
                        //iconImageHref: '',
                        preset:'islands#violetDotIcon',
                        iconImageSize: [32, 32],
                    })

                    myMap.geoObjects
                        .add(placemark)
                });
            });



        // function init() {
        //     const coord = [
        //         {
        //             officeAddress: 'г Ставрополь (Ставропольский край), Ленина 482/1',
        //             OfficeLatitude: 45.038605,
        //             OfficeLongitude: 41.905666
        //         },
        //         {
        //             officeAddress: 'г Ставрополь (Ставропольский край), Ленина 482/2',
        //             OfficeLatitude: 44.038605,
        //             OfficeLongitude: 41.905666
        //         },
        //         {
        //             officeAddress: 'г Ставрополь (Ставропольский край), Ленина 482/3',
        //             OfficeLatitude: 45.038605,
        //             OfficeLongitude: 41.955666
        //         }
        //     ];


        // const myMap = new ymaps.Map("map", {
        //     center: [55.7522, 37.6156],
        //     zoom: 7
        // });

        // coord.forEach(coord => {
        //     const placemark = new ymaps.Placemark([coord.lat, coord.lon], {
        //         hintContent: 'Организация',
        //         balloonContent: coord?.officeAddress
        //     }, {
        //         iconLayout: 'default#image',
        //         iconImageHref: '/img/map_icon.svg',
        //         iconImageSize: [32, 32],
        //         iconImageOffset: [-5, -38]
        //     })

        //     myMap.geoObjects
        //         .add(placemark)
        // });
        //console.log(ymaps.load('https://api-maps.yandex.ru/2.1/?lang=en_US'))
    },
    data() {
        return {
            settings: {
                // apiKey: '',
                lang: 'ru_RU',
                coordorder: 'latlong',
                enterprise: false,
                version: '2.1'
            },
            coordsMap: [55.7522, 37.6156],
            coords: [
                {
                    officeAddress: 'г Ставрополь (Ставропольский край), Ленина 482/1',
                    OfficeLatitude: 45.038605,
                    OfficeLongitude: 41.905666
                },
                {
                    officeAddress: 'г Ставрополь (Ставропольский край), Ленина 482/2',
                    OfficeLatitude: 44.038605,
                    OfficeLongitude: 41.905666
                },
                {
                    officeAddress: 'г Ставрополь (Ставропольский край), Ленина 482/3',
                    OfficeLatitude: 45.038605,
                    OfficeLongitude: 41.955666
                }
            ]
        }
    }
}
</script>

<style scoped>

.map_list_cont{
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.time__map{
    color: grey;
    font-size: 15px;
    font-weight: 400;
}

.map__content {
    border-radius: 30px;

    display: flex;

    overflow: hidden;

    height: 100%;
}

.map__sup{
    color: grey;
    font-size: 15px;
    font-weight: 500;
    margin-top: 0.5rem;
}

.map__content_left {
    background: #fff;

    padding: 30px;

    height: 100%;
}

.map__title {
    font-size: 20px;
    font-weight: 600;
}

.map__list {
    display: flex;
    flex-direction: column;
    row-gap: 10px;

    padding-left: 0;

    overflow: auto;
    margin-top: 1rem;
    font-weight: 600;
}

.ui-map {
    max-height: 710px;
    width: 100%;
    height: 100%;
}
</style>