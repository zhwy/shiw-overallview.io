# Map

## Props

<!-- @vuese:Map:props:start -->
|Name|Description|Type|Required|Default|
|---|---|---|---|---|
|projectId|项目id|`String`|`false`|-|
|autoInit|自动初始化，如果为false，则需要手动调用init方法|`Boolean`|`false`|true|
|layerList|是否显示图层列表|`Boolean`|`false`|false|
|logo|是否显示logo|`Boolean`|`false`|false|
|animationBar|是否显示地图动画控制条|`Boolean`|`false`|false|
|animationList|是否显示动画列表|`Boolean`|`false`|false|
|hideTool|是否隐藏工具栏|`Boolean`|`false`|false|
|defaultHideLayer|图层列表是否默认收起|`Boolean`|`false`|false|
|defaultHideAnimation|动画列表是否默认收起|`Boolean`|`false`|false|
|rightPanel|是否显示右侧面板|`Boolean`|`false`|false|
|pickObject|拾取物体|`Function`|`false`|-|
|pickLayer|拾取图层|`Function`|`false`|-|
|processLayer|处理图层数据|`Function`|`false`|() => {}|
|changeViewerOptsFunc|修改初始化Cesium.Viewer时的参数方法|`Function`|`false`|() => {}|

<!-- @vuese:Map:props:end -->


## Events

<!-- @vuese:Map:events:start -->
|Event Name|Description|Parameters|
|---|---|---|
|loadLayer|开始图层加载，由于图层数据异步获取，此时图层数据可能还未全部加载完毕|-|
|resetProject|重设项目|-|
|loadSuccess|地图初始化完成|-|
|cancelFly|取消飞行|{Object} e 飞行事件|
|layerClick|图层点击事件|{Object} data 图层数据|

<!-- @vuese:Map:events:end -->


## Methods

<!-- @vuese:Map:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|init|获取项目信息并初始化地图|-|
|getLayer|根据关键字获取图层数据|{*} id 图层关键字<br/> {String} key 关键字类型|
|playLayerAnimation|播放图层动画|{String} name 动画名称<br/> {Function} notFound 动画未找到回调<br/> {Function} playParticular 播放特定动画回调<br/> {Function} complete 动画播放完成回调|

<!-- @vuese:Map:methods:end -->


