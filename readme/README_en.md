<!--
 * @Author: yuyanget 845262968@qq.com
 * @Date: 2024-10-18 12:34:50
 * @LastEditors: yuyanget 845262968@qq.com
 * @LastEditTime: 2024-10-24 10:13:54
 * @FilePath: /xy_type/readme/README_en.md
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
# xy_type

- [简体中文](README_zh_CN.md)
- [繁体中文](README_zh_TW.md)
- [English](README_en.md)

# Description
Type tools.

## Source Code Repositories

- <a href="https://github.com/xy-base/xy_type.git" target="_blank">Github</a>  
- <a href="https://gitee.com/xy-base/xy_type.git" target="_blank">Gitee</a>


## Install

```
pip install xy_type
```

## Start

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

## License
xy_type is licensed under the <Mulan Permissive Software License，Version 2>. See the [LICENSE](../LICENSE) file for more info.


## Donate

If you think these tools are pretty good, Can you please have a cup of coffee?  

![Pay-Total](./Pay-Total.png)


## Contact

```
WeChat: yuyangiit
Mail: 845262968@qq.com
```