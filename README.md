# SurveyOnUCMap
“外调助手”是一款基于安卓GIS组件UCMap OpenGL版（源码官网下载地址 http://www.creable.cn/kuibu/xiazai.asp ） 适用于林业、国土、管线以及各类POI点等行业的外业数据采集，
在Google地图上既可以叠加自己的影像图，也可以叠加ShapeFile矢量要素图层，支持对叠加的ShapeFile矢量要素进行编辑，实现对要素图形和属性的采集，
同时，还支持拍照、录音、录像等多媒体功能。
“外调助手”具有以下几个特点：
一、简单易操作；二、通用，各行业都能适用；三、易扩展、可根据不同行业的特殊需求进行扩展定制；四、地图显示速度快，用户体验好。

技术上几点说明：
一、叠加的ShapeFile，需要将ShapeFile拷贝到存储卡根目录下，同时，要求ShapeFile图层的坐标系必须是经纬度，因为Google地图是经纬度坐标的，
如您的ShapeFile不是经纬度坐标，可事先在电脑上用其他软件工具将坐标转成经纬度；
二、叠加的影像，需要事先在电脑上将您的影像tiff进行切片，UCMap提供了切片工具，可将影像tiff切片并存储到sqlite里成为标准的MBTiles格式，
然后将处理好的MBTiles文件拷贝到存储卡根目录下即可，这里，对影像的坐标系没有特别的要求，UCMap提供的切片工具会自动将其他坐标系转成经纬度，
所以，用户不用关心影像的坐标系问题；
三、数据采集，出于对精度的要求，这里采用“打点”模式来绘制点、线、面，“手绘”模式适用于对精度要求不高的数据采集；要素编辑包含图形编辑和属性
编辑，其中图形编辑有节点编辑和裁剪等功能，支持undo、redo功能；
四、定位、轨迹和路径搜索，定位图标指示了当前所在位置，其中图标的箭头指示了手机的朝向，即地图是上北下南，定位箭头的方向便是手机的朝向；
轨迹功能记录了用户行走的路线；路径搜索，调用了天地图的在线接口，返回最优路线；
五、多媒体功能，支持拍照、录音、录像等功能；

以上只是外业数据采集中最通用的功能，您可以参考UCMap OpenGL版开发文档，以及基于该源码做各种修改和扩展，欢迎加入QQ讨论群：543201967；

![Image text](https://github.com/geochenyj/SurveyOnUCMap/blob/master/img-folder/pic1.png)
![Image text](https://github.com/geochenyj/SurveyOnUCMap/blob/master/img-folder/pic2.png)
![Image text](https://github.com/geochenyj/SurveyOnUCMap/blob/master/img-folder/pic3.png)
![Image text](https://github.com/geochenyj/SurveyOnUCMap/blob/master/img-folder/pic4.png)
![Image text](https://github.com/geochenyj/SurveyOnUCMap/blob/master/img-folder/pic5.png)
