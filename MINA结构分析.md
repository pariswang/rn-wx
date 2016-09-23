#MINA结构分析

###1. 入口
app.js    程序逻辑
app.json  配置
app.wxss  样式

###2. 配置
页面配置会覆盖全局配置  
app.json全局配置 
pages: 页面路径 
window: 默认窗口  
tabBar: 底部tab  
networkTimeout: 网络超时 
debug: debug模式 

###3. 页面
一个页面由.json, .js, .wxml, .wxss四个文件组成  
#### * 逻辑层
App注册app  
Page注册页面  
  data初始data 
  onLoad、onReady、onShow、onHide、onUnload 
  setData  

#### * 视图层 
数据绑定 
```{{}}```

条件渲染  
```<view wx:if="{{...}}"></view><view wx:elif="{{...}}"></view>```

列表渲染 
```<view wx:for="{{}}"></view>```

模板 

事件 
tap, touchstart, touchmove, touchcancel, touchend, longtap 

form的submit 
input的input 
scroll-view的scroll 
 

#### * 引用
import 
include 
