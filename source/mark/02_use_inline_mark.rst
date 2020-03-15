.. _topics-02_use_inline_mark:

====
内联标记
====

标准的reST 内联标记
====

- 星号: *text* 是强调 (斜体),
- 双星号: **text** 重点强调 (加粗),
- 反引号: ``text`` 代码样式.

使用限制
    1. 不能相互嵌套
    2. 内容前后不能有空白: 这样写``* text*`` 是错误的

ref  
====

.. code-block:: text

    这个ref就是引用本项目的其他文档的连接的，需要在一个文档的顶部设置
    
        .. _topics-youindex_name:
    
    在另一个文档使用 :ref:`topics-youindex_name`。

doc  
====

:doc:`/base/03_use_list` 

download
====

:download:`/images/panda.jpg` 


替换
====

|release|

|version|

|today|

.. note:: 日期是可以设置日期格式的。
