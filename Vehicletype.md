# 车型接口

接口定义方：唯智

## 功能描述

* CMS模糊查询OWB车型，OWB返回查询结果给CMS。


## 接口详情

路径：

```
    http://14.29.237.141:8090/leaderrun_edi/servlet/leaderrunServiceToCMS/queryBaseVehicleType
```

内容：

```
{
	"code":["CC001","CC002"]   //为空时传"CODE":[]
}
```
返回内容：
```
{
    "contactNumber": "",
    "success": "true",//失败为false
    "content": "成功",
    "status": "1",
    "vehicleTypeInfos": [
        {
            "code": "CC001",//车型编码
            "name": "叉车001",//名称
            "beTrailer": false,//是否挂车
            "transportMode": "汽运",//运输方式
            "fuelType": "",//燃料类型
            "length": 0,//长
            "width": 0,//宽
            "height": 0,//高
            "power": "",//发动机工具
            "volumeLimit": 0,//额定体积
            "weigtLimit": 0,//额定重量
            "crubWeight": 0,//整备质量（千克）
            "description": ""//备注
        }
      ]
    }
   
```
