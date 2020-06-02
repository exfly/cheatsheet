---
title: Go
layout: 2017/sheet
prism_languages: [go, bash]
weight: -3
tags: [Featured]
category: C-like
updated: 2017-09-15
---

## Getting started

{: .-three-column}

### Hello world

{: .-prime}

#### atomic

## compile

- 生成 SSA 整个过程结果展示(html): GOSSAFUNC=hello go build hello/hello.go
- 生成 plan9 汇编代码 GOOS=linux GOARCH=amd64 go tool compile -S hello/hello.go
    - 没有编译优化 GOOS=linux GOARCH=amd64 go tool compile -S -N -l base/array.go
    - -gcflags="-N -l"
- 逃逸分析 go run -gcflags '-m -l' main.go
