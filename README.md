<!--
 * @Author: Violet-VE lolico.violet@gmail.com
 * @Date: 2022-11-13 22:39:53
 * @LastEditors: Violet-VE lolico.violet@gmail.com
 * @LastEditTime: 2022-11-14 01:44:24
 * @FilePath: LearningForUnreal\README.md
 * @Description: README
-->
# LearningForUnreal
Unreal的学习之旅，此分支版本为`5.0.3`
使用本项目内的任何资源素材需遵守 `Apache 2.0` 开源协议。
本人个站    [青冥雅域丨溯堑](https://violet-ve.com/)

## 项目结构说明：

```
- Assets    (存放项目使用到的资源的源文件)
- Config    (项目和编辑器的默认设置)
- Content
    - __ExternalActors__    (UE5开放世界关卡默认创建的目录，对其进行操作会引发不可知的问题，有经验的人可以自行决定)
    - __ExternalObjects__   (同上)
    - Assets    (存放项目中用到的资源，来源网络，按类型分，比如特效的资源放在VFX中，UI的就在UI内。或许会有交叉引用和重复导入的问题，但是查找会方便)
        - VFX   (特效用到的资源)
    - Base  (存放项目的一些基类，新建蓝图的时候能继承的应当从此处继承。后续会视学习内容新增)
        - Blueprints    (蓝图基类)
        - Maps  (关卡基类，新建关卡一般从此新建，后续会视使用频率可能删除)
    - LearningPack  (存放学习成果)
        - VFX   (目前正在学习的特效模块，其余模块按此模板进行创建)
            - Blueprints    (蓝图都放这)
            - UMG   (暂无，放置UI的)
            - Maps  (此模块用到的地图)
            - Cascades  (特效模块的子模块 - 级联粒子)
            - Materials (材质)
            - Niagaras  (最新的Niagara子模块)
- Plugins   (暂无，存放自行开发的插件，使用需遵守协议)
- Source
- LearningForUnreal.uproject
```

## 本项目使用到的商城内可选插件：

1. Property Transfer Tool：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/property-transfer-tool)
    - 此插件可以把一个蓝图中的变量或者函数完整复制到另一个蓝图，可省去繁琐的复制粘贴。不支持跨项目。

2. C++ Module Generator：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/c-module-generator)
    - 此插件可以在编辑器中快速生成模块，可以在插件中生成模块。
    
3. Flat Nodes：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/flat-nodes)
    - 此插件可以美化蓝图节点样式，好看。
    
4. Graph Printer：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/graph-printer)
    - 此插件可以把蓝图节点输出为图片，分享代码时很好用。
    
5. Node Graph Assistant：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/node-graph-assistant)
    - 此插件非常好用，被广大网友所推荐。提高工作效率的利器，使用方法自行百度。
    
6. Restart Editor：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/restart-editor-01)
    - 一键重启编辑器。
    
7. Sirius Utility Nodes：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/sirius-utility-nodes)
    - 提供 `FString` 的格式化功能省去和 `FText` 的相互转换或者繁琐的 `append`
    
8. Switch Language：
    - [商城链接](https://www.unrealengine.com/marketplace/zh-CN/product/switch-language)
    - 点击按钮一键切换中英，非常好用。

## 使用到的自带的插件：

1. Modeling Tools Editor Mode：
    - 理论上现在最新版的UE5新建项目会自带。提供媲美建模软件的建模功能

2. UV Editor：
    - UV编辑器，可以在UE中编辑UV啦！初次进入UV编辑器后直接按`w`可以对UV进行变换操作，还能自动分UV！