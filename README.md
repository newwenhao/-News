**易源News**
================================================================
基于MVP框架，遵循Material Design设计的一款新闻阅读APP和Turing Robot
--------------------------------------------------------------------
#Description
##全篇使用[百度API Store](http://apistore.baidu.com/)的免费API

###**Splash界面**

[loading动画](https://github.com/dinuscxj/LoadingDrawable.git)使用LoadingDrawable开源库

###**新闻资讯页面**
数据所用接口来自百度API Store 的[易源新闻免费API](http://apistore.baidu.com/apiworks/servicedetail/688.html),自定义网络请求工具类
**NetRequestUtil**>**Util**,通Mode层实现**API的JSON数据解析**,Presenter层获取Mode层解析的数据，展示在View层
**界面展示** Fragment容器采用 **CoordinatorLayout**,标签栏采用**TabLayout**，可以横向滚动,Item布局采用**RecycleView**+**SwipeRefreshLayout** +**CardView** 实现卡片式布局 和下拉刷新，上拉加载.通过**Glide**显示图片,点击跳转详情页面时通过**ActivityOptionsCompat**实现图片放大;
通过设置不同channelId 来获取不同频道的新闻

###**开心一刻页面**
只有**文本类和图片类**，获取数据和布局 与新闻资讯一个道理，采用[易源笑话API](http://apistore.baidu.com/apiworks/servicedetail/688.html)**图片类**使用开源框架**PhotoView**支持图片放大

###**Turing聊天页面**
使用[图灵API](http://www.tuling123.com/)提供的API接口,可以回答文本类内容，图片内容，机票内容等等

###天气
数据来源于[和风天气API](http://apistore.baidu.com/apiworks/servicedetail/478.html)，点击跳转详情页面

###**白天，夜间模式**
通过改变主题颜色来实现白天和夜间的切换

##**Library引用**
*  **GSON** Link: [compile 'com.google.code.gson:gson:2.6.2'](http://github.com/google/gson)
*  **Volley** Link: [compile 'com.mcxiaoke.volley:library:1.0.19'](https://github.com/mcxiaoke/android-volley.git)
*  **Glide** Link:[compile 'com.github.bumptech.glide:glide:3.7.0'](https://github.com/bumptech/glide.git)
*  **Loading** Link:[compile 'pl.tajchert:waitingdots:0.2.0'](https://github.com/tajchert/WaitingDots.git)
*  **LogUtils** Link: [compile 'com.apkfuns.logutils:library:1.2.2'](https://github.com/pengwei1024/LogUtils.git)
*  **PhotoView** Link[compile 'com.github.chrisbanes.photoview:library:1.2.4'](https://github.com/chrisbanes/PhotoView.git)
*  **ButterKnife** Link: [compile 'com.jakewharton:butterknife:7.0.1'](http://github.com/jakewharton/butterknife)

##**License**
    Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
