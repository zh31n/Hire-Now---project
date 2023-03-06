<template>
    <VueApexCharts type="line" height="400" :options="options" :series="series"></VueApexCharts>
</template>

<script>
export default {
    data() {
        return {
            options: {
                colors: ["#FF7E7E", "#00A888"],
                grid: {
                    show: false,
                    strokeDashArray: 0,
                    xaxis: {
                        lines: {
                            show: true,
                        },
                    },
                },
                legend: {
                    show: false
                },
                xaxis: {
                    labels: {
                        show: false
                    },
                    axisBorder: {
                        show: false
                    },
                    axisTicks: {
                        show: false
                    }
                },
                dataLabels: {
                    enabled: false
                },
                chart: {
                    toolbar: {
                        show: false
                    },
                    zoom: {
                        enabled: false
                    }
                },
                tooltip: {
                    enabled: false
                },
                toolbar: {
                    show: false
                },
                yaxis: {
                    show: false
                }
            },
        }
    },
    props: {
        series: {
            type: Array
        }
    }
}
</script>