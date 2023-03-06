<template>
    <div class="positions-table">
        <template v-if="!loading">
          <table>
              <thead v-if="headers && headers.length > 0">
                  <tr>
                      <th v-for="(item, index) in headers">{{item.name}}</th>
                  </tr>
              </thead>
              <tbody v-if="items && items.length > 0 && headers && headers.length > 0">
                <tr v-for="(item, index) in items" class="h-14" :class="item.class">
                  <td v-for="(header) in headers" >
                      <template v-if="'key' in header">
                        <slot :name="'item.' + header['key']" :item="item" :index="index">
                          {{ item[ header['key'] ] }}
                        </slot>
                      </template>
                  </td>
                </tr>
              </tbody>
          </table>
        </template>
        <template v-else>
          <div class="loader-wrap">
            <div class="loader">Loading...</div>
          </div>
            <table class="positions__blur">
              <thead>
                  <tr>
                      <th>11dwqdqw wqd</th>
                      <th>111d1112321</th>
                      <th>d21da12323 </th>
                      <th>d2d1</th>
                      <th>d12d 21d2d1</th>
                  </tr>
              </thead>
              <tbody>
                <tr class="h-14" v-for="n in 5">
                  <td>e2e1e21e</td>
                  <td>&ggeg2343432</td>
                  <td>&f32fs</td>
                  <td>10293884</td>
                  <td>kdkwqd123</td>
                </tr>
              </tbody>
            </table>
        </template>
    </div>
      
</template>

<script>
	export default {
	  name: 'Table',
	  components: {  },
	  props: {
	    headers: [],
      items:[],
      loading: true
	  },
	  data() {
	    return {

	    }
	  },
    methods: {
      inputHandler(val) {
        window.console.log(val)

        window.console.log(this.items)
      },
      copy(index) {
        this.items.splice(index, 0, [...this.items[index]]);
      },
      del(index) {
        this.items.splice(index, 1);
      }
    }
	}
</script>

<style scoped>

.tr-dunger td {
  background: #e76f6b38 !important;
}

.img-table {
  max-width: 30px;
  max-height: 40px;
}

/* positions-table  */
.positions-table {
  overflow-x: auto;
  position: relative;
}
.positions-table table {
  width: 100%;
  max-width: 1500px;
  position: relative;
  border-collapse: collapse; 
}

.positions-table__max {
  width: max-content !important;
}

.positions-table th {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  line-height: 18px;
  position: sticky;
  color: #77757D;
  padding: 10px 20px;
      white-space: nowrap;
}
.positions-table tbody tr {
  border: solid #fff 5px;
  border-left: 0px;
  border-right: 0px;
  text-align: left;
}
.positions-table td {
  font-family: 'Montserrat';
  font-style: normal;
  font-weight: 500;
  font-size: 15px;
  line-height: 18px;
    padding: 5px 20px;
  color: #000000;
  background: #F4F4F8;
}

.positions-table td:first-child {
    border-top-left-radius: 20px; 
    border-bottom-left-radius: 20px;
    padding-left: 30px;
}
.positions-table td:last-child {
    border-bottom-right-radius: 20px; 
    border-top-right-radius: 20px; 
    padding-right: 30px;
}

.positions-table th:first-child {
  padding-left: 30px;
}
.positions-table th:last-child {
  padding-right: 30px;
}
.positions-table thead tr {
  text-align: left;
}

.positions__blur {
  filter: blur(8px);
}

/* positions-table end  */


.loader-wrap {
  overflow: hidden;
  position: absolute;
  z-index: 10;
  left: 0px;
  top: 0px;
  width: 100%;
  height: 100%;
}


.loader {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 11em;
  height: 11em;
  border-radius: 50%;
  background: #92e6d6;
  background: -moz-linear-gradient(left, #92e6d6 10%, rgba(146,230,214, 0) 42%);
  background: -webkit-linear-gradient(left, #92e6d6 10%, rgba(146,230,214, 0) 42%);
  background: -o-linear-gradient(left, #92e6d6 10%, rgba(146,230,214, 0) 42%);
  background: -ms-linear-gradient(left, #92e6d6 10%, rgba(146,230,214, 0) 42%);
  background: linear-gradient(to right, #92e6d6 10%, rgba(146,230,214, 0) 42%);
  position: relative;
  -webkit-animation: load3 1.4s infinite linear;
  animation: load3 1.4s infinite linear;
  -webkit-transform: translateZ(0);
  -ms-transform: translateZ(0);
  transform: translateZ(0);
}
.loader:before {
  width: 50%;
  height: 50%;
  background: #92e6d6;
  border-radius: 100% 0 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}
.loader:after {
  background: #ffffff;
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}
@-webkit-keyframes load3 {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(360deg);
    transform: rotate(360deg);
  }
}
@keyframes load3 {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(360deg);
    transform: rotate(360deg);
  }
}

</style>