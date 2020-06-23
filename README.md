# LeqiAnalyticsSDK

### How to use LeqiAnalyticsSDK
   * pod 'LeqiAnalyticsSDK'*

   ```
   //进行上传地址的填写
   + (void)startWithServerURL:(NSString *)urlString;    
   举例：[LeqiAnalyticsSDK startWithServerURL:@"https://big-data.leqi.us/api/test/event/ios"];
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
