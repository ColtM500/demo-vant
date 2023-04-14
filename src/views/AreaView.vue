<template>
  <div>
    <van-area title="标题" :area-list="areaList"
    @confirm="showArea" />
  </div>
</template>

<script>
// const areaList = {
//   province_list: {
//     110000: '北京市',
//     120000: '天津市',
//     130000: '河北省',
//   },
//   city_list: {
//     110100: '北京市',
//     120100: '天津市',
//     130100: '石家庄市',
//     130200: '唐山市',
//   },
//   county_list: {
//     110101: '东城区',
//     110102: '西城区',
//     120101: '河东区',
//     120102: '河西区',
//     130101: '长安区',
//     130102: '桥西区',
//     130201: '路南区',
//     130202: '路北区',
//     // ....
//   },
// };

//从下载好的全国省市区数据库包中提取数据，命名为areaList
import {areaList} from '@vant/area-data'

export default {
  data() {
    return { areaList };
  },
  methods:{
    showArea(area){
      console.log("选择地址的信息", area)
    },
  }
};
</script>

<style scoped>

</style>