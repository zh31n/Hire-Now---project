<template>
	<div>
		<no-ssr> 
			<VueApexCharts max-width="300" type="area" :options="chartOptions" :series="series"></VueApexCharts>
		</no-ssr>
	</div>
</template>

<script>
	export default {
	  name: 'WeekChart',
	  components: {  },
		props: {
			weekData: {}
		},
		computed: {
		  series: function () {
		    return [{
					name: 'Прошлая неделя',
					data: this.weekData.last
				},{
					name: 'Текщая неделя',
					data: this.weekData.current
				}]
		  }
		},
	  data() {
	    return {
			chartOptions: {
					chart: {
	          height: 350,
	          type: 'area',
						zoom: {
							enabled: false
						},
				    locales: [{
				      "name": "ru",
				      "options": {
				        "shortDays": ["Сб", "Вс", "Пн", "Вт", "Ср", "Чт", "Пт" ],
				      }
				    }],
				    defaultLocale: "ru"
	        },
	        dataLabels: {
	          enabled: false
	        },
	        stroke: {
	          curve: 'smooth'
	        },
	        xaxis: {
	          categories: ["Сб", "Вс", "Пн", "Вт", "Ср", "Чт", "Пт" ]
	        },
			colors:['#D9D9D9', '#92E6D6'],
			legend: {
				show: false
			}
				},
	    }
	  },
	}
</script>

<style scoped>

</style>