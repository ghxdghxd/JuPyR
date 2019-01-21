---
Title: julia 用法
Date: 2019/1/4 10:23:41
Modified: 2019/1/4 10:23:41
Category: 小抄速查
Tags: julia
Slug: julia-summary
Authors: JT Guo
Summary: julia 用法简介
---
# julia 语法

```julia
DataFrames, mapcols

```

## 不支持的

1.`～`不能代表HOME
2.字符串不能使用`'`
    单引号为Char
    双引号为String

## 文件是否存在

```julia
isfile(file)
```

## 加载RData

```julia
using RData
dat = load("RData")
```

### 加载“R非data.frame”, 丢失行列名，

```julia
dat = load("RData", convert = F)
```

|R|python|julia|
|---|---|---|
