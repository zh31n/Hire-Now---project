<template>
	<div>

		<div class="content-title">Отчеты</div>

		<div class="grid grid-cols-2 gap-4 mt-12">
        <div class="report-box report-box_color_1">
            <a href="report_1.php" class="report-box__link">Отчет о выкупленных товарах ></a>
        </div>
        <div class="report-box report-box_color_2">
            <a href="report_1.php" class="report-box__link">Отчет о забраных товарах ></a>
        </div>
        <div class="report-box report-box_color_3">
            <a href="report_1.php" class="report-box__link">Отчет об опубликованных отзывах ></a>
        </div>
        <div class="report-box report-box_color_4">
            <a href="report_1.php" class="report-box__link">Товары на нашем складе ></a>
        </div>
		</div>

		<div class="mt-7">
			<a href="/reports.php" class="content-link-all">К полному отчету</a>
		</div>

	</div>
</template>

<script>
	export default {
	  name: 'Reports',
	  components: {  },
	  data() {
	    return {
	      
	    }
	  },
	}
</script>

<style scoped>
/* report-box  */
.report-box {
  width: 100%;
  height: 156px;
  
  border-radius: 25px;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  align-items: flex-end;
  position: relative;
}

.report-box__desc {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 55px;
  color: #FFFFFF;
  position: absolute;
  left: 0px;
  bottom: -13px;
  width: 100%;
  display: block;
  text-align: center;
}

.report-box.report-box_content {
  max-width: 354px;
  height: 251px;
  align-items: flex-start;
}

.report-box.report-box_color_1 {
  background: #F9E1E1;
}
.report-box.report-box_color_2 {
  background: #E6F2E3;
}
.report-box.report-box_color_3 {
  background: #E5EAFD;
}
.report-box.report-box_color_4 {
  background: #FCEDCB;
}
.report-box__link {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  color: #000000;
}
/*  report-box end */
</style>