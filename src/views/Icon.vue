<template>
  <div>
    <div class="crumbs">
      <el-breadcrumb separator="/">
        <el-breadcrumb-item><i class="el-icon-ali-18"></i> 自定义图标</el-breadcrumb-item>
      </el-breadcrumb>
    </div>
    <div class="container">
      <h2>使用方法</h2>
      <p style="line-height: 50px;">
        直接通过设置类名为 el-icon-ali-iconName 来使用即可。例如：（共{{iconList.length}}个图标）
      </p>
      <p class="example-p">
        <i
          class="el-icon-ali-hongbao"
          style="font-size: 30px;color: #ff5900"
        ></i>
        <span>&lt;i class=&quot;el-icon-ali-hongbao&quot;&gt;&lt;/i&gt;</span>
      </p>
      <p class="example-p">
        <i
          class="el-icon-ali-weibo"
          style="font-size: 30px;color:#fd5656"
        ></i>
        <span>&lt;i class=&quot;el-icon-ali-weibo&quot;&gt;&lt;/i&gt;</span>
      </p>
      <p class="example-p">
        <i
          class="el-icon-ali--smiling-"
          style="font-size: 30px;color: #ffc300"
        ></i>
        <span>&lt;i class=&quot;el-icon-ali--smiling-&quot;&gt;&lt;/i&gt;</span>
      </p>
      <br>
      <h2>图标</h2>
      <div class="search-box">
        <el-input
          class="search"
          size="large"
          v-model="keyword"
          clearable
          placeholder="请输入图标名称"
        ></el-input>
      </div>
      <ul>
        <li
          class="icon-li"
          v-for="(item,index) in list"
          :key="index"
        >
          <div class="icon-li-content">
            <i :class="`el-icon-ali-${item}`"></i>
            <span>{{item}}</span>
          </div>
        </li>
      </ul>
    </div>

  </div>
</template>

<script>
export default {
    data: function() {
        return {
            keyword: '',
            iconList: [
                'icon-test',
                'icon-test1',
                'icon-test2',
                'icon-test3',
                'icon-test4',
                'icon-test5',
                'icon-test6',
                'icon-test7',
                'icon-test8',
                'icon-test9',
                'icon-test10',
                'icon-test11',
                'icon-test12',
                'icon-test13',
                'icon-test14',
                'icon-test15',
                'icon-test16',
                'icon-test17',
                'icon-test18',
                'icon-test19',
                'icon-test20',
                'icon-test21',
                'icon-test22',
                'icon-test23',
                'icon-test24',
                'icon-test25',
                'icon-test26',
                'icon-test27',
                'icon-test28',
                'icon-test29',
                'icon-test30',
                'icon-test31',
                'icon-test32',
                'icon-test33',
                'icon-test34',
                'icon-test35',
                'icon-test36',
                'icon-test37',
                'icon-test38',
                'icon-test39',
                'icon-test40',
                'icon-test41',
                'icon-test42',
                'icon-test43',
                'icon-test44',
                'icon-test45',
                'icon-test46',
                'icon-test47',
                'icon-test48',
                'icon-test49',
                'icon-test50',
                'icon-test51',
                'icon-test52',
                'icon-test53',
                'icon-test54',
                'icon-test55',
                'icon-test56',
                'icon-test57',
                'icon-test58',
                'icon-test59',
                'icon-test60',
                'icon-test61',
                'icon-test62',
                'icon-test63',
                'icon-test64',
                'icon-test65',
                'icon-test66',
                'icon-test67',
                'icon-test68',
                'icon-test69',
                'icon-test70',
                'icon-test71',
                'icon-test72',
                'icon-test73',
                'icon-test74',
                'icon-test75',
                'icon-test76',
                'icon-test77',
                'icon-test78',
                'icon-test79',
                'icon-test80',
                'icon-test81',
                'icon-test82',
                'icon-test83',
                'icon-test84',
                
            ]
        };
    },
    computed: {
        list() {
            return this.iconList.filter(item => {
                return item.indexOf(this.keyword) !== -1;
            });
        }
    }
};
</script>

<style scoped>
.example-p {
    height: 45px;
    display: flex;
    align-items: center;
}
.search-box {
    text-align: center;
    margin-top: 10px;
}
.search {
    width: 300px;
}
ul,
li {
    list-style: none;
}
.icon-li {
    display: inline-block;
    padding: 10px;
    width: 120px;
    height: 120px;
}
.icon-li-content {
    display: flex;
    height: 100%;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}
.icon-li-content i {
    font-size: 36px;
    color: #606266;
}
.icon-li-content span {
    margin-top: 10px;
    color: #787878;
}
</style>