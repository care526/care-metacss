# 原子类文档

## 整体的设计规范
fw  
mg-t_20  
fs_20  
属性-描述_值  
描述和值不一定同时存在  

## 项目结构  
- docs              文档
- metas             源代码目录
  - modules         模块
    - flex          flex
    - float         浮动
    - font          文字、排版
    - margin        margin
    - padding       padding
    - position      position
  - index           主文件
  - vars            全局变量

## 一些简化的描述代表什么
1. -t => top
2. -b => bottom
3. -l => left
4. -r => right

5. -v => 竖向
6. -h => 横向

...

## 一些简化的值代表什么
具体的值代表什么还是要看前面的描述是什么  
1. _s => flex-start
2. _c => center
3. _e => flex-end
4. _sb => space-between
5. _sa => space-around

6. _r => relative
7. _a => absolute
8. _f => fixed
9. _s => sticky

...

## 所有简化对应的具体css
### flex
```css
flex1 => flex: 1;
row => display: flex;
/* 一行排列 横 纵 对其的方式 */
row-v_s
row-v_c
row-v_e
row-v_sb
row-v_sa

row-h_s
row-h_c
row-h_e
row-h_sb
row-h_sa
/* 换行 */
row-wp_w => flex-wrap: wrap;
row-wp_wr => flex-wrap: wrap-reverse;
```
将row替换为column 就是竖轴排列，描述属性同上
### float
```css
fl => float: left;
fr => float: right;
```
### font
- 字体大小
  ```css
  fs_20 => font-size: 20px;
  ```
- 行高
  ```css
  lh_20 => line-height: 20px;
  ```
- 字重
  ```css
  fw => font-weight: bold;
  fwer => font-weight: bolder;
  fw_700 => font-weight: 700;
  ```
- 对齐
  ```css
  ta_l => text-align: left;
  ta_c => text-align: center;
  ta_r => text-align: right;
  ```

### height width
```css
h_1 => height: 1px;
```
width同height
### margin padding
```css
mg-t_1 => margin-top: 1px;
mg-b_1 => margin-bottom: 1px;
mg-l_1 => margin-left: 1px;
mg-r_1 => margin-right: 1px;
mg-v_a => margin: auto 0;
mg-h_a => margin: 0 auto;
```
padding同margin  
### position
```css
pt_r => position: relative;
pt_a => position: absolute;
pt_f => position: fixed;
pt_s => position: sticky;
t_1 => top: 1px;
b_1 => bottom: 1px;
l_1 => left: 1px;
r_1 => right: 1px;
```
