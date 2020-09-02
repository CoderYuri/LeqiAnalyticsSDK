# LeqiAnalyticsSDK

### How to use LeqiAnalyticsSDK
   //pod 'LeqiAnalyticsSDK'  暂不可用

   ```
   #import <LeqiAnalyticsSDK/LeqiAnalyticsSDK.h>

   //进行上传地址的填写
   + (void)startWithServerURL:(NSString *)urlString;    
   
   请求URL： https://big-data.leqi.us/api/<app_key>/event/ios  生产环境
   app_key为该应用的标识
   APP KEY  产品备注
   9e66e6c0  智能证件照
   ca81b25c  最美
   d0c02ba2  证件照制作
   d41ba5c2  乐骐证件照在线拍摄
   e09f591a  长宽相机
   
   在AppDelegate文件中  进行初始化操作
   举例：[LeqiAnalyticsSDK startWithServerURL:@"https://big-data.leqi.us/api/e09f591a/event/ios"];
   ```
   
   ```
   //提交用户user_id
   - (void)login:(NSString *)loginId;      
   举例：[[LeqiAnalyticsSDK sharedInstance] login:@"user_id"];
   ```
   
   ```
   //自定义埋点
   - (void)track:(NSString *)eventName;    
   举例：[[LeqiAnalyticsSDK sharedInstance] track:@"click"];
   ```
   
   ```
   //leqidata_black_list
   leqidata_black_list.plist文件  
   将不用统计的控制器添加进来  就可以不统计该页面
   ```
