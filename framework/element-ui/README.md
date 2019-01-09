# ElementUI

vue2.0的Element UI的表格table 格式化 把数字格式化成文字


 <el-table-column prop="casestatus" label="是否结案"  width="100px" :formatter="ifendcase" >
      </el-table-column>

在el-table里直接加一个formatter，绑定一个方法

在methods中加入

   ifendcase(val){
      console.log("aaaaaa");
      console.log(val.casestatus);

       if(val.casestatus == '1 ')
      {return "是"}
        else if (val.casestatus == '0')
        {return "否"}
        else
        {return "进行中"}
    },

直接return即可，不需要加入row, column 等参数
