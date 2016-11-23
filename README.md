本工程为基于高德地图iOS SDK进行封装，实现了building显隐的控制。
## 前述 ##
- [高德官网申请Key](http://lbs.amap.com/dev/#/).
- 阅读[开发指南](http://lbs.amap.com/api/ios-sdk/summary/).
- 工程基于iOS 3D地图SDK实现

## 功能描述 ##
基于3D地图SDK，可以控制building显示与隐藏。

## 核心类/接口 ##
| 类    | 接口  | 说明   | 版本  |
| -----|:-----:|:-----:|:-----:|
| MAMapView	| BOOL showsBuildings | 是否显示楼块，默认为YES | v4.0.0 |

## 核心难点 ##

```
/* switch事件回调. */
- (void)actionBuilding:(UISwitch *)sender
{
    self.mapView.showsBuildings = sender.on;
}
```