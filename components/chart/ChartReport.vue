<template>
    <VueApexCharts type="area" height="100%" :options="options" :series="series"></VueApexCharts>
</template>

<script>
export default {
    data() {
        return {
            options: {
                legend: {
                    position: 'top',
                    markers: {
                        radius: 0,
                        width: 40,
                        height: 20,
                    }
                },
                colors: ["#6290FE", "#9A9A9A"],
                fill: {
                    colors: ["transparent", "transparent"],
                    gradient: {
                        gradientToColors: ['#6592ff', '#fff'],
                        opacityFrom: 1,
                        opacityTo: 0.87,
                        //inverseColors: true,
                        type: "vertical"
                        // linear-gradient(180deg, rgba(101, 146, 255, 0.8) 0%, #FFFFFF 86.98%)
                    },
                    type: 'gradient'
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
                    size: 3,
                    strokeWidth: 1,
                },
                yaxis: [
                    {
                        // opposite: true,
                        axisTicks: {
                            show: true
                        },
                        axisBorder: {
                            show: true,
                            color: "#57a0e4"
                        },
                        labels: {
                            style: {
                                colors: "#57a0e4"
                            }
                        }
                    },
                    {
                        show: false,
                    }
                ],
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