---
layout: post
title: Camera【threejs】[API]
keywords: Sign,Sign的博客,技术文章,web开发,threejs中文API
description: 将官网的api翻译为中文
tags: [threejs, web]
---
##摄像头Camera

摄像头对象的基础类，但你创建一个新的摄像头对象时，这个类将被继承。

###构造函数

Camera()

构造函数将matrixWorldInverse和projectionMatrix设定到正确的类型。

###属性

.matrixWorldInverse

matrixWorld的逆反矩阵，matrixWorld是摄像头在全局内变换时的矩阵参数。

.projectionMatrix

投影矩阵。

###方法

.getWorldDirection (vector)

vector — (可选项)

这个方法返回一个表示摄像头在全局内朝向的向量对象。

.lookAt ( vector )

vector — 指向的点

在全局内只要摄像头在场景的(0,0,0)位置，镜头方向就会被指向向量点所在的位置

.clone ( camera )

camera — 复制摄像头

这个方法返回摄像头的复制对象。

###源码

<a href="https://github.com/mrdoob/three.js/blob/master/src/cameras/Camera.js" target="_blank">https://github.com/mrdoob/three.js/blob/master/src/cameras/Camera.js</a>

####附：

涉及到的api

<a href="http://threejs.org/docs/index.html#Reference/Core/Object3D" target="_blank">Object3D（英文地址，中文更新中）</a>

<a href="http://threejs.org/docs/index.html#Reference/Math/Matrix4" target="_blank">Matrix4（英文地址，中文更新中）</a>

<a href="http://threejs.org/docs/index.html#Reference/Math/Vector3" target="_blank">Vector3（英文地址，中文更新中）</a>