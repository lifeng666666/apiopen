# apiopen  免费开放接口API

> - http://www.apiopen.top/  开源社区地址
> - http://www.apiopen.top/api.html  所有接口文档
> - https://binaryify.github.io/NeteaseCloudMusicApi/#/   网易云音乐 NodeJS 版 API 在GitHub上的API
> - https://github.com/lifeng666666/KindleHelper  小说API 此项目中有追书神器上的一些暴露的API等
> - http://www.bejson.com/knownjson/webInterface/  JSON API免费接口
> - https://www.free-api.com/ https://github.com/fangzesheng/free-api
> - https://github.com/MZCretin/RollToolsApi 一个提供开发中常用数据的一个稳定聚合Api接口源，运行于独立服务器，免费，且长期维护，会持续添加新的接口！
> - https://github.com/wulh8410/WebAPI 公共应用免费API接口
> - https://github.com/insoxin/API  https://api.isoyu.com/#/ 

# api的平台

- https://www.apishop.net
- https://www.alapi.cn

### 电商接口

- 淘宝商品搜索建议:

  http://suggest.taobao.com/sug?code=utf-8&q=商品关键字&callback=cb  

  ps:callback是回调函数设定



### 物流接口

- 快递接口:

  http://www.kuaidi100.com/query?type=快递公司代号&postid=快递单号  

  ps:快递公司编码:申通="shentong" EMS="ems" 顺丰="shunfeng" 圆通="yuantong" 中通="zhongtong" 韵达="yunda" 天天="tiantian" 汇通="huitongkuaidi" 全峰="quanfengkuaidi" 德邦="debangwuliu" 宅急送="zhaijisong"

### 谷歌接口

- FeedXml转json接口:

  http://ajax.googleapis.com/ajax/services/feed/load?q=Feed地址&v=1.0 [用例(请右击在新窗口打开)](http://ajax.googleapis.com/ajax/services/feed/load?q=http://www.bilibili.tv/rss-13.xml&v=1.0)[官方文档](https://developers.google.com/feed/v1/jsondevguide#resultJson)

  备选参数:callback：&callback=foo就会在json外面嵌套foo({})方便做jsonp使用。 
  备选参数:n：返回多少条记录。

### 百度接口

- 百度百科接口:

  http://baike.baidu.com/api/openapi/BaikeLemmaCardApi?scope=103&format=json&appid=379020&bk_key=关键字&bk_length=600[用例(请右击在新窗口打开)](http://baike.baidu.com/api/openapi/BaikeLemmaCardApi?scope=103&format=json&appid=379020&bk_key=银魂&bk_length=600)

  查询出错示例如下：查看原始页面 {"error_code":"20000","error_msg":"search word not found"}

### 天气接口

- 百度接口:

  http://api.map.baidu.com/telematics/v3/weather?location=嘉兴&output=json&ak=5slgyqGDENN7Sy7pw29IUvrZ [用例](http://www.oschina.net/code/snippet_554046_35134)[官方文档](http://developer.baidu.com/map/carapi-7.htm)

  location:城市名或经纬度 ak:开发者密钥 output:默认xml

- 气象局接口:

  http://m.weather.com.cn/data/101010100.html [解析](http://blog.csdn.net/zgyulongfei/article/details/7956118) [用例](http://bejson.com/demos/weather.php)

- 

  新浪接口:

  http://php.weather.sina.com.cn/iframe/index/w_cl.php?code=js&day=0&city=&dfc=1&charset=utf-8 [用例](http://www.bejson.com/demo/sinaweather/)

  参数中city如果给了参数就是相关的城市,否则会自动判断
  day=0的话是今天 
  返回的参数 大家看着办吧,具体的我也不清楚,新浪没给API。

### 音乐接口

- QQ空间音乐接口

  http://qzone-music.qq.com/fcg-bin/cgi_playlist_xml.fcg?uin=QQ号码&json=1&g_tk=1916754934[用例](http://bejson.com/demos/qqmusic/) [代码解释和下载](http://www.jqdemo.com/932.html)

- QQ空间收藏音乐接口

  http://qzone-music.qq.com/fcg-bin/fcg_music_fav_getinfo.fcg?dirinfo=0&dirid=1&uin=QQ号&p=0.519638272547262&g_tk=1284234856

- 多米音乐接口

  http://v5.pc.duomi.com/search-ajaxsearch-searchall?kw=关键字&pi=页码&pz=每页音乐数

- soso接口

  http://cgi.music.soso.com/fcgi-bin/fcg_search_xmldata.q?source=10&w=关键字&perpage=1&ie=utf-8

### 视频信息接口[JSON在线工具](http://www.bejson.com/)

- 优酷

  http://v.youku.com/player/getPlayList/VideoIDS/视频ID (比如 http://v.youku.com/v_show/id_XNTQxNzc4ODg0.html的ID就是XNTQxNzc4ODg0)

- 爱奇艺

  http://cache.video.iqiyi.com/jp/avlist/202861101/1/?callback=jsonp9

- 土豆接口

  http://api.tudou.com/v3/gw?method=album.item.get&appKey=Appkey&format=json&albumId=视频剧集ID&pageNo=当前页&pageSize=每页显示 [示例(火影忍者剧集)](http://api.tudou.com/v3/gw?method=album.item.get&appKey=myKey&format=json&albumId=Lqfme5hSolM&pageNo=5&pageSize=100) [官方文档](http://api.tudou.com/apidoc/index.php/剧集节目查询)

  http://www.tudou.com/tvp/getMultiTvcCodeByAreaCode.action?type=3&app=4&codes=Lqfme5hSolM&areaCode=320500&jsoncallback=__TVP_getMultiTvcCodeByAreaCode [示例(火影忍者APP剧集)](http://www.tudou.com/tvp/getMultiTvcCodeByAreaCode.action?type=3&app=4&codes=Lqfme5hSolM&areaCode=320500&jsoncallback=__TVP_getMultiTvcCodeByAreaCode)

### 地图接口

- 阿里云根据地区名获取经纬度接口

  http://gc.ditu.aliyun.com/geocoding?a=苏州市 [官方文档](http://ditu.aliyun.com/jsdoc/geocode_api.html)

  参数解释: 纬度,经度 type 001 (100代表道路，010代表POI，001代表门址，111可以同时显示前三项)

- 阿里云根据经纬度获取地区名接口

  http://gc.ditu.aliyun.com/regeocoding?l=39.938133,116.395739&type=001 [官方文档](http://ditu.aliyun.com/jsdoc/geocode_api.html)

- 获取用户的IP,国家代码缩写,经纬度

  http://www.telize.com/geoip?callback=a [测试用例](http://www.telize.com/geoip?callback=cb)

  参数解释: callback是回调函数

- 获取用户经纬度，以及获取附近建筑物名/span>

  http://ditu.amap.com/service/pl/pl.json?rand=635840524184357321[测试用例](http://ditu.amap.com/service/pl/pl.json?rand=635840524184357321)

  http://ditu.amap.com/service/regeo?longitude=121.04925573429551&latitude=31.315590522490712[测试用例](http://ditu.amap.com/service/regeo?longitude=121.04925573429551&latitude=31.315590522490712)

### IP接口

- 新浪接口(ip值为空的时候 获取本地的)

  http://int.dpool.sina.com.cn/iplookup/iplookup.php?format=json&ip=218.4.255.255

- 淘宝接口

  http://ip.taobao.com/service/getIpInfo.php?ip=63.223.108.42

### 手机信息查询接口 [JSON在线工具](http://www.bejson.com/)

- 淘宝网接口

  http://tcc.taobao.com/cc/json/mobile_tel_segment.htm?tel=手机号

- 拍拍接口

  http://virtual.paipai.com/extinfo/GetMobileProductInfo?mobile=手机号&amount=10000&callname=getPhoneNumInfoExtCallback [用例](http://bejson.com/demos/paipai-tel.php)

- 百付宝接口

  https://www.baifubao.com/callback?cmd=1059&callback=phone&phone=手机号

- 115接口

  http://cz.115.com/?ct=index&ac=get_mobile_local&callback=jsonp1333962541001&mobile=手机号

- 有道接口

  http://www.youdao.com/smartresult-xml/search.s?jsFlag=true&type=mobile&q=手机号

- 手机在线接口

  http://api.showji.com/Locating/www.showji.com.aspx?m=手机号&output=json&callback=querycallback

### 翻译、词典接口

- 腾讯

  http://dict.qq.com/dict?q=词语

### 腾讯的部分接口

- 获取QQ昵称和用户头像

  http://r.qzone.qq.com/cgi-bin/user/cgi_personal_card?uin=QQ(不过是jsonp哦)
