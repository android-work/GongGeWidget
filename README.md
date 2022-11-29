# GongGeWidget
  宫格控件

  #控件集成：
  在工程的build.gradle中添加如下代码
  allprojects {
  repositories {
  ...
  maven { url 'https://jitpack.io' }
}
}

  在模块的build.gradle中添加依赖
  dependencies {
	        implementation 'com.github.android-work:GongGeWidget:v1.0.1'
	}


# 布局中引用：
  1、宽高wrap_content，表示父控件最大限制为屏幕宽高

  2、direction：表示排版方向，start 左对齐/上对齐；end 右对齐/下对齐；between 等大小均分某方向尺寸

  3、column：列数，只在orientation：horizontal 且 direction：between 生效

  4、row：行数，只在orientation：vertical 且 direction：between 生效

  5、orientation：horizontal 水平方向；vertical 垂直方向

  6、horizontalSpace：水平间距

  7、verticalSpace：垂直间距

  <com.android.work.widgetmodel.widget.GongGeWidget
  android:id="@+id/gongGe"
  android:layout_width="wrap_content"
  android:layout_height="wrap_content"
  android:background="#fffccfff"
  app:direction="start"
  app:horizontalSpace="10dp"
  app:orientation="horizontal"
  app:verticalSpace="10dp">

  ....子控件

  </com.android.work.widgetmodel.widget.GongGeWidget
 
 ## 测试控件功能窗口
![测试控件功能窗口](https://user-images.githubusercontent.com/40420651/204466174-0bafd437-b7ad-458b-9806-e570339fd747.jpg)

## 垂直排版，下对齐
![垂直排版，下对齐](https://user-images.githubusercontent.com/40420651/204466708-4cd15c40-0d88-4dba-b0d5-dc6f71bc17bc.jpg)

## 垂直排版，上对齐
![垂直排版，上对齐](https://user-images.githubusercontent.com/40420651/204466225-f21efae7-ddf1-435b-ab84-eea21a1d930b.jpg)

## 水平排版，右对齐
![水平排版，右对齐](https://user-images.githubusercontent.com/40420651/204466248-0c123e2d-4041-42b1-adb5-73a1af105907.jpg)

## 水平排版，左对齐
![水平排版，左对齐](https://user-images.githubusercontent.com/40420651/204466275-bce9d0c3-a6bb-47a6-aed4-0cf35ac16abd.jpg)

## 水平等分宽度
![水平等分宽度](https://user-images.githubusercontent.com/40420651/204466311-ac2c24c6-0fdd-481a-80f4-6d630dccda20.jpg)

