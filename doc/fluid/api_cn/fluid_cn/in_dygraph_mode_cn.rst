.. _cn_api_fluid_in_dygraph_mode:

in_dygraph_mode
-------------------------------

.. py:function:: paddle.fluid.in_dygraph_mode()

该接口检查程序是否在动态图模式中运行。
可以通过 ``fluid.dygraph.guard`` 接口开启动态图模式。

返回：如果程序是在动态图模式下运行的，则返回 ``True``。

返回类型：bool

**示例代码**

.. code-block:: python

    import paddle.fluid as fluid

    fluid.enable_dygraph()          # 现在进入 dygragh 模式
    print(fluid.in_dygraph_mode())  # True
    fluid.disable_dygraph()
    print(fluid.in_dygraph_mode())  # False


