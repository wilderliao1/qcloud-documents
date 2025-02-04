# Release Notes - Web

## 2.1.0 @ 2019.05.29
新增功能
- 支持预加载，白板初始化增加参数：preloadDepth用于指定图片预加载深度，默认值为5（表示预加载当前页前后5页的图片）
- 笔迹优化，白板初始化增加参数：smoothLevel用于指定笔迹平滑级别，默认值0.1，取值[0, 1]
- 支持禁止数据同步，白板初始化增加参数：dataSyncEnable用于指定是否启用数据同步，同时增加对应的接口setDataSyncEnable、isDataSyncEnable
- 橡皮擦工具支持滑动擦除，没有接口变更
- TEduBoardWarningCode新增一个TEDU_BOARD_WARNING_H5PPT_ALREADY_EXISTS = 3的枚举值，当要添加的H5PPT已存在时抛出该警告
- 文档展示优化，支持独立设置白板宽高比，支持滑动缩放


| 新增初始化参数	| 类型	| 必填 | 默认值 |说明
--------- | --------- | ----- | --------- | --------- |
| boardContentFitMode | Number | 否 | 0 | 0 不自动调整白板宽高比，文件等比例缩放居中显示，文件宽高<=白板宽高<br/> 1 自动调整白板宽高比与文件一致，文件铺满白板，白板等比例缩放居中显示，白板宽高<=容器宽高<br/> 2 自动调整白板宽高比与文件一致，文件铺满白板，白板等比例缩放居中显示，白板宽高>=容器宽高 |
| dataSyncEnable | Boolean | 否 | true | 是否数据同步 |
| scale | Number | 否 | 100 | 实际缩放比为scale/100 |
| preloadDepth | Number | 否 | 5 | 预加载深度，预加载前后preloadDepth页白板 |
| smoothLevel | Number | 否 | 0.1 | 平滑级别，取值0～1之间的浮点数，0表示不启用平滑 |



| 新增接口          | 说明      |
| ------------------ | ---------------------------------------- |
| setBoardRatio                            |          设置当前的白板比例                           |
| getBoardRatio                            |          获取当前的白板比例                           |
| setBoardScale                                  |          设置当前的白板缩放比                           |
| getBoardScale                            |          获取当前的白板缩放比                           |
| setDataSyncEnable                            |          设置是否同步数据                           |
| isDataSyncEnable                            |          获取是否允许同步数据                           |
| setBoardContentFitMode                            |          设置白板文件的显示方式                           |
| getBoardContentFitMode                            |          获取白板文件的显示方式                           |

## 2.0.0.2 @ 2019.05.22

1. bug修复
    - 文字输入在mac中的兼容性问题
    - 修复PPT动画在iphone显示异常的问题

## 2.0.0.1 @ 2019.05.15

1. 新增功能支持：
    - 白板
        - 新增鼠标工具类型TEDU_BOARD_TOOL_TYPE_MOUSE
        - 支持设置H5背景
        - 白板支持并发文件上传
2. bug修复
    - 新增白板有边框


## 2.0.0_RC3 @ 2019.05.10

1. 新增功能支持：
    - 白板
        - 支持设置文本样式及字体属性
        - 初始化接口支持传入所有属性初始值
        - 初始化支持设置白板宽高比
        - `AddFile` 接口支持传入COS转码URL


## 2.0.0_RC2 @ 2019.05.08

1. 新增功能支持：
    - 白板
        - 涂鸦（铅笔、橡皮、激光教鞭、直线、空心椭圆、空心矩形、实心椭圆、实心矩形、文本）
        - 背景色、背景图
        - 点选、框选、移动涂鸦、撤销、重做
        - 白板缩放、移动
        - 文件展示（静态：支持PPT、PDF、WORD、EXCEL）、多文件支持
        - PPT动画展示
