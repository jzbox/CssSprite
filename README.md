# CssSprite
-
一、简述作用

使用compass的sprite方法进行图片的合并，通过固定的配置代码，方便地进行sprite图的生成。

二、setting.scss文件的固定设置

@charset "utf-8";
// 配置sprite间距
$setting-spacing: 10px;

// 配置sprite的布局方式：horizontal/vertical/smart
$setting-layout: vertical;

// 设置false不自动清除过期的sprite
$setting-clean-up: false;

// 配置sprite的位置
//$setting-position: 0px;

// 自动输出尺寸
$setting-sprite-dimensions: true;

@import "compass/css3";
@import "compass/utilities/sprites";
@import "setting/*.png";
@include all-setting-sprites;
