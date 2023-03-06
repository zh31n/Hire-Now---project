<template>
	<div>
		<client-only> 
			<template v-if="toggle">
				<carousel
					:margin="10"
					:responsiveClass="true"
					:dots="true"
					:nav="false"
					:responsive="{0:{items:2},600:{items:3},1000:{items:5}}"
				>
					<template v-for="(item, index) in fastinfo">
						<div class="fast-info-item">
				  <div class="fast-info-item__title">
					  {{item.value}}
					  
					  <span class="fast-info-help" v-if="item.help">?</span>

				  </div>
				  <div class="fast-info-item__desc">{{item.label}}</div>
				  <template v-if="item.link">
					  <Button class="rounded-lg p-2.5 but-1" >{{item.link_name}}</Button>
				  </template>
			  </div>
					</template>
				</carousel>
			</template>
		</client-only>
	</div>
</template>

<script>
export default {
  name: 'Fastinfo',
  components: {  },
  data() {
	return {
	  fastinfo: [],
	  toggle: false
	}
  },
  methods: {
	getFastInfo() {
	  this.$store.dispatch('request/get_fastinfo').then((x) => {
				this.fastinfo = x.data.items
		  this.$nextTick(() => {
			this.toggle = true;
		  });
	  })
	},
  },
  mounted() {
   this.getFastInfo()
  },
}
</script>


<style scoped>
.fast-info-item {
  height: 150px;
  background: #FFFFFF;
  border-radius: 15px;
  padding: 15px;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  justify-content: center;
  flex-grow: 2;
  gap: 10px;
  margin: 5px;
}

.fast-info-item__title {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  color: #000000;
		display: flex;
		align-items: center;
		justify-content: space-between;
}
.fast-info-item__desc {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #76767D;
  margin-top: 5px;
}
.fast-info-item__but {
  margin-top: 16px;
}
.fast-info-help {
  display: inline-block;
  background: #f0f0f2;
  color: #4e4e53;
  width: 26px;
  height: 26px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  position: relative;
}
</style>