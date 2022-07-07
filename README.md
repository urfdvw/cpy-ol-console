# CircuitPython Online Console
This repo is supposed to be part of the project [CircuitPython Online IDE](https://github.com/urfdvw/CircuitPython-online-IDE) (mentioned as CPy OL IDE below).
In the upcoming first numbered version CPy OL IDE,
this repo should become a github sub-module.

# Propose of this repo
- Provide a more refined version of the CircuitPython Console
- Practice using Vue and JS
    - Make a reusable app that can be used stand alone and also with an Editor app in the future

# Features (TODO List)
- 可控的串口
    - 可选波特率
    - 完整的串口生命周期
        - 有断开和重联的选项
- 目前全部的功能
    - 命令窗历史
    - 键盘快捷键
- 可以检测当前状态
    - Repl 还是运行
- 可以检测哪一部分是输入，哪一部分是输出
- 视觉美化
    - 将输入代卖和输出结果分开在不同的方块中显示
        - 如同 jupyter note book
    - 运行时输入的命令用另外的方式显示
    - 输入方块加入几个按键
        - 再次运行
        - 编辑后再次运行
- 插件
    - 运作方式
        - 使用 python 库包装输出命令
            - 比如占位符 `{{type: plot, x-axis:false}}`
        - 在JS里接受命令并生成或操作插件
    - 种类
        - 数据可视化插件
            - 图表插件：绘制点线图
            - 仪表插件：仅绘制最新值
        - 控件
            - 用于输入值
                - 形式：滚动条，下拉菜单等等
                - 更新方法：按键发送，自动发送
            - 自动 deactive 过期的插件
        - 单步调试插件
- 留出接口供编辑器调用
                