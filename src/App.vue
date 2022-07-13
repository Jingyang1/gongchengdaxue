<template>

<!-- 头部区域 -->
  <div class="header">
    <div class="toushang">
     <a href="#" class="toubua">回到首页</a><span>丨</span><a href="#" class="toubua">ENGLISH</a>
    </div>
    <div class="headerx">
      <div class="touxia">
        <div class="touxial"><a href="#"><img src="./img/logo.png" alt="logo"></a></div>
        <div class="sousuoniu"><el-button type="primary" icon="el-icon-search"></el-button></div>
        <div class="touxiar"><el-input v-model="input" placeholder="请输入内容"></el-input>
        <br><br><a href="#" class="toubub">网上服务办事大厅</a>
        </div>
      </div>
    </div>
     
  <!-- 导航区域 -->
  <div class="daohang"><el-row :gutter="10">
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao"><span class="el-dropdown-link">
        学校概况</span></a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">院部设置</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">组织机构</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">人才培养</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">科学研究</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">学科建设</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">师资力量</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">招生就业</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">国际交流</a></div></el-col>
      <el-col :span="2"><div class="dao1"><a href="#" class="xuexiao">校园生活</a></div></el-col>
      </el-row>
  </div>
  <div class="lunbo">
    <el-carousel>
    <a href="#"><el-carousel-item v-for="item in 1" :key="item" height="375px">
      <img src="./img/0FCE48555DEFB3B2CD1DDC046EB_A6128690_1D7A0.jpg" alt="" width="1530px" >
    </el-carousel-item></a>
    <a href="#"><el-carousel-item v-for="item in 1" :key="item" height="375px">
      <img src="./img/1185BEB7AC96E8E60CD8588C78D_2D17547F_1676C.jpg" alt="" width="1530px">
    </el-carousel-item></a>
    <a href="#"><el-carousel-item v-for="item in 1" :key="item" height="375px">
      <img src="./img/7C74EBE1796A21BA8DEFC13AFB6_2D7FB905_3F3C6.jpg" alt="" width="1530px">
    </el-carousel-item></a>
    <a href="#"><el-carousel-item v-for="item in 1" :key="item" height="375px">
      <img src="./img/A99E5939BD86CB1204E57631703_0878C32B_14790.jpg" alt="" width="1530px">
    </el-carousel-item></a>
  </el-carousel>
  </div>

  </div>
 

</template>

<script>
export default {
  data() {
    return {
      input: '',
      
    }
  },
  methods(){
   
  }
}
</script>

<style lang="scss" scoped>
 @import './css/index.css';
 .header{
  height: 30px;
  background-color: rgb(181, 5, 28);
   border-bottom: 1px solid rgb(255, 255, 255);
 };
 .toushang{
  width: 1200px;
  height: 30px;
  margin: auto;
 
 };
 .toubua{
  color: aliceblue;
  font-size: 12px;
 };
 .headerx{
  height: 160px;
  background-color: rgb(181, 5, 28);
  border-bottom: 1px solid rgb(255, 255, 255);
 };
 .touxia{
  width: 1200px;
  height: 160px;
  margin: auto;
  padding-top: auto;
 };
 .touxial{
  padding-top: 20px;
  float: left;
 }
 .touxiar{
  float: right;
  width: 300px;
  padding-top: 40px;
  color: aliceblue;
 }
 .toubub{
  color: aliceblue;
  float: right;
 }
 .sousuoniu{
  float: right;
  padding-top: 40px;
  color: burlywood;
 }
 .daohang{
  height: 50px;
  background-color: rgb(255, 255, 255);
  padding-left: 190px;
 }
  .el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 2px;
   
  }
  .dao1{
    line-height: 50px;
    padding-left: 20px;
  }
  .xuexiao{
    color: darkred;
  }
  .lunbo{
   width: 1530px;
   height:375px
  }
</style>
