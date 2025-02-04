# Release Notes - Android

## 2.1.0 @ 2019.05.29
1. 白板
    - 支持图片预加载功能；
    - 支持是否将涂鸭数据同步给其他端功能；
    - 优化涂鸭笔迹去锯齿，让线条变得更平滑；
    - 优化橡皮擦工具，支持滑动擦除;
    - 优化H5ppt错误提示，在H5ppt文件已经存在的情况下抛出警告;
    - 优化文档展示，支持独立设置白板宽高比，支持滑动缩放;；

## 2.0.0.2 @ 2019.05.22
1. 白板
    - 修改BUG；

## 2.0.0.1 @ 2019.05.15

1. 新增功能支持：
    - 白板
        - 新增使用网页作为白板的背景；
        - 新增工具鼠标的功能，可以方便的手势翻页；
2. 问题修复
    - 修正Demo中白板的构建方式，移到TIC SDK中统一初始和反初始化；

## 2.0.0_RC3 @ 2019.05.10

1. 新增功能支持：
    - 白板
        - 支持设置文本样式及字体属性
        - 初始化接口支持传入所有属性初始值
        - 初始化支持设置白板宽高比
        - `AddFile` 接口支持传入COS转码URL
2. 问题修复
    - Demo依赖的IM版本指定为4.3.81，修复最新版IM修改接口导致编译异常问题


## 2.0.0_RC2 @ 2019.05.08

1. 新增功能支持：
    - 白板
        - PPT动画展示
3. 新增服务：
    - PPT动画转码服务


## 2.0.0_RC1 @ 2019.04.26

1. 新增功能支持：
    - 音视频通信
        - 实时音视频通信
        - 屏幕分享/播片（可与摄像头画面并存）
    - 云通信
        - 消息
        - 群组
        - 关系链管理
    - 白板
        - 涂鸦（铅笔、橡皮、激光教鞭、直线、空心椭圆、空心矩形、实心椭圆、实心矩形、文本）
        - 背景色、背景图
        - 点选、框选、移动涂鸦、撤销、重做
        - 白板缩放、移动
        - 文件展示（静态：支持PPT、PDF、WORD、EXCEL）、多文件支持
