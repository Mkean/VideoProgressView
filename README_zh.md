# LightProgressView + VolumeProgressView
![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
[Englist](https://github.com/zhangchaojiong/VideoProgressView/edit/master/README.md) | [中文版本](https://github.com/zhangchaojiong/VideoProgressView/edit/master/README_zh.md)
>一种创意的亮度动画，可通过上下滑动来控制手机屏幕的亮度。 动画从太阳（白天是明亮的）到月亮（夜晚是黑暗的）变化，一个非常漂亮的屏幕亮度动画！

## 效果演示：
![2020-05-03 01_00_28.gif](https://upload-images.jianshu.io/upload_images/2788235-f057d49c96baa63d.gif?imageMogr2/auto-orient/strip)

![2020-05-05 18_09_07.gif](https://upload-images.jianshu.io/upload_images/2788235-cd0a98eda6c1c711.gif?imageMogr2/auto-orient/strip)


## 如何使用：
* 加入 gradle 依赖

```
implementation 'com.cj.videoprogressview:progressview:1.0.0'
```
* 在 xml 加入相应的动画:

```
<com.cj.videoprogressview.LightProgressView
        android:id="@+id/lpv"
        android:padding="10dp"
        android:background="@drawable/bg_center_window"
        android:layout_width="88dp"
        android:layout_height="88dp"
        app:lpv_halo_color="@android:color/white"
        app:lpv_moon_color="@android:color/white"
        app:lpv_halo_height="7dp"
        app:lpv_halo_width="2dp"/>
```

```
<com.cj.videoprogressview.VolumeProgressView
        android:id="@+id/vpv"
        android:layout_marginLeft="3dp"
        android:padding="10dp"
        android:background="@drawable/bg_center_window"
        android:layout_width="88dp"
        android:layout_height="88dp"
        app:vpv_halo_color="@android:color/white"
        app:vpv_halo_height="7dp"
        app:vpv_halo_width="2dp"
        />
```

## 可使用的参数解析 
LightProgressView 自定义参数：
```
   <declare-styleable name="LightProgressView">
        //光晕的长度
        <attr format="dimension" name="lpv_halo_height"/> 
        //光晕的厚度
        <attr format="dimension" name="lpv_halo_width"/>
        //光晕的个数
        <attr format="integer" name="lpv_num_of_halo"/>
        //拟合圆的值，默认是0.43f，越大月亮弯曲度越大
        <attr format="float" name="lpv_magicnum"/>
        //月亮的颜色
        <attr format="color" name="lpv_moon_color"/>
        //光晕的颜色
        <attr format="color" name="lpv_halo_color"/>
    </declare-styleable>
```
VolumeProgressView 自定义参数：
```

    <declare-styleable name="VolumeProgressView">
    //光晕的长度
        <attr format="dimension" name="vpv_halo_height"/>
        //光晕的厚度
        <attr format="dimension" name="vpv_halo_width"/>
        //光晕的个数
        <attr format="integer" name="vpv_num_of_halo"/>
        //自定义低音量时的图片
        <attr format="integer" name="vpv_volume_low"/>
         //自定义中等音量时的图片
        <attr format="integer" name="vpv_volume_medium"/>
     //自定义高音量时的图片
        <attr format="integer" name="vpv_volume_high"/>
        //光晕的颜色
        <attr format="color" name="vpv_halo_color"/>
    </declare-styleable>
```

## 详细解析
* [wiki](https://www.jianshu.com/p/55e7de12451d) 
* [博客地址](https://www.jianshu.com/p/55e7de12451d) 

## 版权声明

```
Copyright (C) 2020 chaojiong.zhang

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```