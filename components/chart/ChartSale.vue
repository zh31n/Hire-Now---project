<template>
    <VueApexCharts type="area" height="100%" :options="options" :series="series"></VueApexCharts>
</template>

<script>
export default {
    data() {
        return {
            options: {
                border: {
                    show: true,
                    colors: ['#000']
                },
                legend: {
                    horizontalAlign: 'right',
                    position: 'top',
                    fontSize: '15px',
                    fontFamily: "'Montserrat', sans-serif",
                    fontWeight: 700,
                    markers: {
                        fillColors: ['transparent', 'transparent'],
                        strokeColor: 'transparent',
                        width: 44,
                        height: 14,
                        customHTML: function () {
                            return `<label class="checkbox-google">
                                        <input type="checkbox" checked>
                                        <span class="checkbox-google-switch"></span>
                                    </label>`
                        }
                    }
                },
                colors: ["#6290FE", "#9A9A9A"],
                fill: {
                    colors: ["transparent", "transparent"],
                    gradient: {
                        gradientToColors: ['#6592ff', '#fff'],
                        opacityFrom: 1,
                        type: "vertical"
                    },
                    type: 'gradient'
                },
                grid: {
                    show: false,
                },
                chart: {
                    toolbar: {
                        show: false
                    },
                    zoom: {
                        enabled: false
                    }
                },
                markers: {
                    show: false,
                },
                xaxis: {
                    axisBorder: {
                        show: true,
                        color: '#000',
                        height: 1,
                        width: '100%',
                    }
                },
                yaxis: {
                    axisTicks: {
                        show: true
                    },
                    axisBorder: {
                        show: true,
                        width: 1,
                        color: "#000"
                    },
                    labels: {
                        style: {
                            colors: "#000"
                        }
                    }
                },
                // stroke: {
                //     show: true,
                //     curve: 'smooth',
                //     lineCap: 'butt',
                //     colors: ['#000'],
                //     width: 2,
                // }
            },
        }
    },
    props: {
        series: {
            type: Array
        },
        categories: {
            type: Array
        }
    },
    mounted() {
        if (this.categories) {
            this.options = {
                ...this.options,
                xaxis: {
                    categories: this.categories
                }
            }
        }
    }
}
</script>

<style>
.checkbox-google {
    display: inline-block;
    height: 28px;
    line-height: 28px;
    margin-right: 10px;
    position: relative;
    vertical-align: middle;
    font-size: 14px;
    user-select: none;
}

.checkbox-google input+.checkbox-google-switch {
    background: #9ABEF7;
    display: inline-block;
    width: 36px;
    height: 14px;
    border-radius: 20px;
    position: relative;
    top: 6px;
    vertical-align: top;
    transition: .2s;
}

.checkbox-google input+.checkbox-google-switch:before {
    background: #1a73e8;
    border-radius: 50%;
    box-shadow: 0 3px 1px -2px rgba(0, 0, 0, 0.2), 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12);
    transition: .15s;
    content: '';
    display: inline-block;
    width: 20px;
    height: 20px;
    position: absolute;
    top: -3px;
    left: -1px;
    transform: translateX(18px);
}

.apexcharts-inactive-legend .checkbox-google .checkbox-google-switch {
    background: #9f9f9f;
    transition: .15s;
}

.apexcharts-inactive-legend .checkbox-google .checkbox-google-switch:before {
    background: #fff;
    transform: translateX(0);
    transition: .15s;
}

.checkbox-google input {
    display: block;
    width: 0;
    height: 0;
    position: absolute;
    z-index: -1;
    opacity: 0;
}

/* Disabled */
/* .checkbox-google input:disabled+.checkbox-google-switch {
    filter: grayscale(60%);
    border-color: rgba(0, 0, 0, .1);
}

.checkbox-google input:disabled+.checkbox-google-switch:before {
    background: #eee;
} */
</style>