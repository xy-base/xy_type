<!--
 * @Author: yuyanget 845262968@qq.com
 * @Date: 2024-10-18 12:34:50
 * @LastEditors: yuyanget 845262968@qq.com
 * @LastEditTime: 2024-10-24 10:14:22
 * @FilePath: /xy_type/README.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
# xy_type

- [简体中文](readme/README_zh_CN.md)
- [繁体中文](readme/README_zh_TW.md)
- [English](readme/README_en.md)

# 说明
类型工具.

## 源码仓库

- <a href="https://github.com/xy-base/xy_type.git" target="_blank">Github地址</a>  
- <a href="https://gitee.com/xy-base/xy_type.git" target="_blank">Gitee地址</a>

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

## 许可证
xy_type 根据 <木兰宽松许可证, 第2版> 获得许可。有关详细信息，请参阅 [LICENSE](LICENSE) 文件。

## 捐赠

如果小伙伴们觉得这些工具还不错的话，能否请咱喝一杯咖啡呢?  

![Pay-Total](./readme/Pay-Total.png)


## 联系方式

```
微信: yuyangiit
邮箱: 845262968@qq.com
```