# CssSprite

### 一、简述作用<br />

使用compass的sprite方法进行图片的合并，通过固定的配置代码，方便地进行sprite图的生成。

### 二、setting.scss文件的固定设置<br />

    @charset "utf-8";
    // 配置sprite间距
    $setting-spacing: 10px;
    
    // 配置sprite的布局方式：horizontal/vertical/smart
    $setting-layout: horizontal;
    
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

### 三、使用操作<br />
通过改变配置sprite的布局方式，生成水平排列或垂直排列的图片。<br />

1、只支持合并.png格式图片；

2、合并元素按命名顺序排列（以纯数字命名）；

3、合并时，先将同类型图片水平排列，最后将所有水平图片垂直排列合并效果最佳；



