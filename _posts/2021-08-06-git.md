---
date: 2021-08-06 00:00:00
layout: post
title: GIT筆記
subtitle: 檔案的時光機，好git，不用嗎?
description: 我是描述
image: https://i.imgur.com/bN14QAC.png
optimized_image: https://i.imgur.com/bN14QAC.png
category: tools
tags:
  - tools
  - git
  - tips
author: tuna
---
# GIT筆記

[TOC]
## Git .gitignore - 忽略特定檔案

### 
### 已經上傳檔案後反悔想要忽略此檔案
> 如果檔案已經上git並且被push上repo 但後續發現這檔案不想要被追蹤(like:env) 
在補上.gitignore後還是沒消失 使用以下指令移除這個檔案的追蹤
- 檔案
```
git rm --cached <file>
```
- 資料夾
```
git rm -r --cached <folder>
```

[參考](https://stackoverflow.com/questions/1274057/how-can-i-make-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitign)

## Git Branch
### 重新命名Git Branch
假設現在有兩個 branch， master 跟 old-branch ，目前在 master ，想要把 old-branch 的名字改成 new-branch 的話，請輸入：
```shell
git branch -m old-branch new-branch
```
如果現在已經在 old-branch ，想要直接把名字改成 new-branch 的話，就輸入：
```shell
git branch -m new-branch
```
[參考](https://fredchiu.wordpress.com/2011/12/28/%E9%87%8D%E6%96%B0%E5%91%BD%E5%90%8D-rename-git-branch/)

