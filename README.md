# LeqiAnalyticsSDK

### How to use LeqiAnalyticsSDK
#### pod 'LeqiAnalyticsSDK'



、、、
+ (void)startWithServerURL:(NSString *)urlString;    //进行上传网址的填写
举例：
[LeqiAnalyticsSDK startWithServerURL:@"https://big-data.leqi.us/api/test/event/ios"];

- (void)login:(NSString *)loginId;      //提交用户user_id
举例：
[[LeqiAnalyticsSDK sharedInstance] login:@"user_id"];

- (void)track:(NSString *)eventName;    //自定义埋点
[[LeqiAnalyticsSDK sharedInstance] track:@"click"];
、、、
