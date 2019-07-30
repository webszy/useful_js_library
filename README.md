# useful_js_library
useful Javascript Library when i on work (工作中常用的js库，以及相关函数)

### 函数类

+ 处理数字为逗号分隔

  ```javascript
  parseNum(num) {
    // 数字每三位加逗号
    return (num || 0).toString().replace(/(\d)(?=(?:\d{3})+$)/g, '$1,')
  }
  ```

  

### 工具库

+ 动画库  [lottie-web](https://github.com/airbnb/lottie-web)
+ css动画   [animate.css](https://github.com/daneden/animate.css)
+ 文件下载  [file-saver](https://github.com/eligrey/FileSaver.js)
+ h5视频播放   [vue-video-player](https://github.com/surmon-china/vue-video-player)
+ 下拉刷新，上拉加载 [mescroll](https://github.com/mescroll/mescroll)
+ 移动端看console [vconsole](https://github.com/Tencent/vConsole)
+ Stripe组件 [vue-stripe-elements-plus](https://github.com/fromAtoB/vue-stripe-elements)
+ MD5 (blueimp-md5)[https://github.com/clearbladeplatform/blueimp_md5]
+ plist
+ xlsx

### UI库

+ 移动端 [vant](https://github.com/youzan/vant)
+ totast & loading [vue2-toast](https://github.com/lin-xin/vue-toast)
+ 表格 [d2-crud](https://github.com/d2-projects/d2-crud)
