# 原子类文档

## 整体的设计规范
属性-方向_值  
```css
/* mg-top_20 */
{
  margin-top: 20px;
}
/* row-v_c */
{
  display: flex;
  item-align: center;
}
```

## 项目结构  
- index
- vars
  - modules
    - flex
    - float
    - font
    - margin
    - padding
    - position


## - 代表什么
对应的属性的额外描述  
1. -v  竖向
2. -h  横向

## _ 代表什么
对应属性的值的简称  
具体还是和对应的属性相关联，一般是值的第一个字母  
例子：
1. _t     top
2. _b     bottom
3. _r     right
4. _l     left
5. _20    20px 20
