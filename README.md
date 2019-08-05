# useful_js_library
useful Javascript Library when i on work (工作中常用的js库，以及相关函数)

### 函数类

+ 处理数字为逗号分隔

  ```javascript
  function parseNum(num) {
    // 数字每三位加逗号
    return (num || 0).toString().replace(/(\d)(?=(?:\d{3})+$)/g, '$1,')
  }
  ```
+ 获取get时的parameter

  ```javascript
  function getURLParams(str){
    let q={}
    str.replace(/([^?&=]+)=([^&]+)/g,(_,k,v)=>q[k]=v)
    return q
  }
  ```
+ 捕获await的错误

  ```javascript
    function to(promise) {
      return promise
          .then(data => {
              return [null, data];
          })
          .catch(err => [err]);
  }
  ```
+ 判断游览器信息(来自网络)

  ```javascript
    function BrowserType() {
      const ua = navigator.userAgent.toLowerCase();
      const testUa = regexp => regexp.test(ua);
      const testVs = regexp => (ua.match(regexp) + "").replace(/[^0-9|_.]/ig, "").replace(/_/ig, ".");
      // 接上以上if...else条件判断
      // ......
      // 获取到system、systemVs、platform、engine、engineVs、supporter、supporterVs、shell、shellVs
      return Object.assign({
          engine, // webkit gecko presto trident
          engineVs,
          platform, // desktop mobile
          supporter, // chrome safari firefox opera iexplore edge
          supporterVs,
          system, // windows macos linux android ios
          systemVs
      }, shell === "none" ? {} : {
          shell, // wechat qq uc 2345 sougou liebao maxthon baidu
          shellVs
      });
  }

  ```
  + 获取本月天数
  
  ```javascript
  function GetDaysOfMonth(Year,Month){
    var date = new Date(Year, Month, 0);
     return(parseInt(date.getDate()));
  }
  ```

### 工具库

+ svg动画  [lottie-web](https://github.com/airbnb/lottie-web)
+ css动画   [animate.css](https://github.com/daneden/animate.css)
+ 文件下载  [file-saver](https://github.com/eligrey/FileSaver.js)
+ h5视频播放   [vue-video-player](https://github.com/surmon-china/vue-video-player)
+ 下拉刷新，上拉加载 [mescroll](https://github.com/mescroll/mescroll)
+ 移动端看console [vconsole](https://github.com/Tencent/vConsole)
+ Stripe支付组件 [vue-stripe-elements-plus](https://github.com/fromAtoB/vue-stripe-elements)
+ MD5 [blueimp-md5](https://github.com/clearbladeplatform/blueimp_md5)
+ 构建ios的plist [plist](https://github.com/TooTallNate/plist.js)
+ 解析xlsx  [xlsx](https://github.com/SheetJS/js-xlsx)

### UI库

+ 移动端 [vant](https://github.com/youzan/vant)
+ totast & loading [vue2-toast](https://github.com/lin-xin/vue-toast)
+ 表格 [d2-crud](https://github.com/d2-projects/d2-crud)
+ 图表: [echarts,地图在map文件夹中](https://github.com/apache/incubator-echarts)

### 未来方向

#### 前端
+ typescript+React
+ dart & flutter

#### 后端
+ nodejs的继续深入
+ rust 
