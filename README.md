# Flag-Guard-Team-Management-System


#项目说明：
    组员：李安为24051106 、金翀昊24150136
    项目内容：高校国旗护卫队信息管理移动端app
    过程记录：AI提示词（包括调试提问，已省略部分重复内容）：
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
  12、操作时PS C:\Users\Ivan1\Documents\HBuilderProjects\GH> mkdir -p src/styles


    目录: C:\Users\Ivan1\Documents\HBuilderProjects\GH\src


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----          2025/5/1     16:47                styles


PS C:\Users\Ivan1\Documents\HBuilderProjects\GH> touch src/styles/variables.scss
touch : 无法将“touch”项识别为 cmdlet、函数、脚本文件或可运行程序的名称。请检查名称的拼写，如果包
括路径，请确保路径正确，然后再试一次。
所在位置 行:1 字符: 1
+ touch src/styles/variables.scss
+ ~~~~~
    + CategoryInfo          : ObjectNotFound: (touch:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
怎么办
  13、PS C:\Users\Ivan1\Documents\HBuilderProjects\GH> npm install --force
npm warn using --force Recommended protections disabled.
npm error code ETARGET
npm error notarget No matching version found for @dcloudio/vite-plugin-uni@^2.0.0-31920230418001.
npm error notarget In most cases you or one of your dependencies are requesting
npm error notarget a package version that doesn't exist.
npm error A complete log of this run can be found in: C:\Users\Ivan1\AppData\Local\npm-cache\_logs\2025-05-01T08_25_36_615Z-debug-0.log
  14、报错16:21:29.476 [plugin:vite:vue]  ../../../../../Documents/HBuilderProjects/GH/App.vue: At least one <template> or <script> is required in a single file component.
16:21:29.486 at App.vue:1:0
16:21:29.565 [plugin:uni:app-nvue-app-style] Could not load ./app.css.js (imported by ../../../../../Documents/HBuilderProjects/GH/main.js): At least one <template> or <script> is required in a single file component.
16:21:29.574 at App.vue:1:0


#环境配置：
本程序使用HBuilder搭建编写，需使用HBuilder打开。
本项目使用网易MuMu模拟器构建安卓虚拟机进行运行测试。
本项目需要在HBuilder中安装的组件为：uView Plus、uni-calendar、uni-datetime-picker	、uni-tag
本项目需要在HBuilder中安装的插件为：APP真机运行、dart-sass编译、scss/sass编译、uni-app（x）（Vue3）、uni-helpers、uni-modules插件、uniCloud本地调试运行插件、uts编辑器、内置终端
（注：HBuilder具有运行的代码时自动根据代码内容提示下载和安装对应插件的功能）


#运行方式：
    启动网易MuMu模拟器后，选择并配制安卓移动端环境，将代码源码文件下载后，安装H Builder并使用H Builder打开文件，index.vue即为主程序代码。需先对h builder进行网易模拟器的适应性配置，配置链接如下https://xiaoshen.blog.csdn.net/article/details/134394974?sharetype=blogdetail&amp;sharerId=134394974&amp;sharerefer=WAP&amp;sharesource=，然后选择菜单栏运行点击运行到手机或模拟器选择运行到Android APP基座，找到系统识别到的模拟机，选择运行代码，即可在电脑端进行本项目移动端APP可视化运行。
