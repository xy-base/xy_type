<!--
 * @Author: yuyangit yuyangit.0515@qq.com
 * @Date: 2024-10-18 12:34:50
 * @LastEditors: yuyangit yuyangit.0515@qq.com
 * @LastEditTime: 2024-10-24 10:13:25
 * @FilePath: /xy_type/readme/README.zh-hant.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
# xy_type

- [简体中文](../README.md)
- [繁體中文](README.zh-hant.md)
- [English](README.en.md)

# 说明
類型工具.

## 程式碼庫

- <a href="https://github.com/xy-base/xy_type.git" target="_blank">Github位址</a>  
- <a href="https://gitee.com/xy-opensource/xy_type.git" target="_blank">Gitee位址</a>  
- <a href="https://gitcode.com/xy-opensource/xy_type.git" target="_blank">GitCode位址</a>  

## 安装
```
pip install xy_type
```

## 开始

```python
from xy_type.utils import count_of_function_arguments, validate_callable_func, validate_callable_init_func, has_func, empty_value

class xyObject:

    def __init__(self, arg_0=0, arg_1=1):
        pass

    def xyFunc(self, arg_0=0, arg_1=1):
        pass

    @classmethod
    def xyClsFunc(cls, arg_0=0, arg_1=1)
        pass

count_of_function_arguments(xyObject.xyClsFunc)
# 2

validate_callable_func(xyObject.xyClsFunc)
# True

validate_callable_init_func(xyObject, 1)
# True

obj = xyObject()
has_func(obj, "xyFunc", 2)
# True
has_func(obj, "xyFunc1", 2)
# False
has_func(obj, "xyFunc", 20)
# False

empty_value(obj, xyObject, None)
# obj

empty_value(obj, str, None)
# None

```

## 許可證
xy_type 根據 <木蘭寬鬆許可證, 第2版> 獲得許可。有關詳細信息，請參閱 [LICENSE](../LICENSE) 文件。

## 捐贈

如果小夥伴們覺得這些工具還不錯的話，能否請咱喝一杯咖啡呢?  

![Pay-Total](./Pay-Total.png)

## 聯繫方式

```
微信: yuyangiit
郵箱: yuyangit.0515@qq.com
```