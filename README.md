# LYPickerChiceView
封装的UIPickerView
选择填写个人资料
# 效果图
![](https://github.com/liuyik/LYPickerChiceView/blob/master/效果图.gif)

## 根据枚举来显示选择类型
//数据类型枚举
typedef NS_ENUM(NSInteger, DATATYPE) {
    LYPickerDataCustom,//自定义
    LYPickerDataGender,//性别
    LYPickerDataHeight,//身高
    LYPickerDataWeight,//体重
    LYPickerDataSalary,//工资
    LYPickerDataDete,//时间
    LYPickerDataArea//地点
};
## 用法


```
//创建
_picker = [[LYPickerChiceView alloc] initWithFrame:self.view.bounds];
            _picker.dataType = LYPickerDataArea;
            _picker.delegate = self;
            [self.view addSubview:_picker];
//协议
- (void)PickerSelectorIndixInfo:(NSDictionary *)info {
    /*
     * 判断类型；
     * 时间类型字典的key为year、month、day；
     * 地点类型字典key为province、city、area；
     * 其他，字典key为：info；
     */    
 }
```





