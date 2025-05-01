# Flag-Guard-Team-Management-System


#项目说明：
    组员：李安为24051106 、金翀昊24150136
    项目内容：高校国旗护卫队信息管理移动端app
    过程记录：AI提示词：
    1、uniapp实现：高校国旗护卫队信息管理app，由以下六个页面构成，可通过主界面的选择按钮进行切换：1.军装信息统计，包括每件的军装种类（海、陆、空）、军装尺码（帽子、上衣、裤子尺码分别记录）、损坏部位、借出人姓名，所有信息可手动录入  2.马靴信息统计，包括马靴尺码、损坏部位  3.团队大事件及安排日历  4.每周一大型升旗排班记录（包括信息：当天日期，主旗姓名，护旗姓名，拉旗姓名，马刀手姓名，队列多名人员姓名名单，后勤多名人员姓名名单，主持人姓名，拍照人员姓名名单） 5.点名界面（带训人员手动点击确认每个人到场），可手动录入删除训练人员姓名表   6.设置军装检索系统，可通过不同的军装信息检索军装，以此快捷找到所有符合条件的军装  要求页面尽量精美
    2、index.vue页面代码
    3、确保已正确安装uView Plus组件库，具体应如何实现安装及检查
    4、为何运行后点击相应模块无法进入界面
    5、项目目录结构中pages文件下的index文件与uniform、boots、schedule等文件是并列关系吗
    6、[Object] {"errMsg":"navigateTo:fail page `/pages/uniform/index` is not found"}  at pages/index/index.vue:139”
    7、第一条回答中的各个模块具体的实现内容如“<template>
  <view class="form-container">
    <u-form :model="form" ref="uForm">
      <u-form-item label="军种类型">
        <u-radio-group v-model="form.type">
          <u-radio name="海军" shape="circle"></u-radio>
          <u-radio name="陆军" shape="circle"></u-radio>
          <u-radio name="空军" shape="circle"></u-radio>
        </u-radio-group>
      </u-form-item>
      
      <u-form-item label="尺码信息">
        <u-input v-model="form.size.hat" placeholder="帽子尺码" />
        <u-input v-model="form.size.coat" placeholder="上衣尺码" />
        <u-input v-model="form.size.pants" placeholder="裤子尺码" />
      </u-form-item>

      <u-button type="primary" @click="saveUniform">保存信息</u-button>
    </u-form>

    <u-table :data="uniformList">
      <!-- 表格展示列 -->
    </u-table>
  </view>
</template>”，应该插入在主index文件中index.vue的什么位置
  8、配置easycom自动导入中{
  "easycom": {
    "autoscan": true,
    "custom": {
      "^u--(.*)": "uview-plus/components/u-$1/u-$1.vue",
      "^up-(.*)": "uview-plus/components/u-$1/u-$1.vue"
    }
  }
}放在原有内容的什么位置
  9、找不到vite.config.js和node_modules怎么办
  10、创建 vite.config.js在什么位置
  11、主程序运行报错：16:10:19.172 [plugin:vite:vue]  ../../../../../Documents/HBuilderProjects/GH/App.vue: At least one <template> or <script> is required in a single file component.
16:10:19.195 at App.vue:1:0
16:10:20.353 [plugin:uni:app-nvue-app-style] Could not load ./app.css.js (imported by ../../../../../Documents/HBuilderProjects/GH/main.js): At least one <template> or <script> is required in a single file component.
16:10:20.375 at App.vue:1:0


#环境配置：
