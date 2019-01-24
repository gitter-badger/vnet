[![Build Status](https://travis-ci.org/rc452860/vnet.svg?branch=master)](https://travis-ci.org/rc452860/vnet)
[![Go Report Card](https://goreportcard.com/badge/github.com/rc452860/vnet)](https://goreportcard.com/report/github.com/rc452860/vnet) [![Join the chat at https://gitter.im/kitami-vnet/community](https://badges.gitter.im/kitami-vnet/community.svg)](https://gitter.im/kitami-vnet/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

<img src="./assert/donate.png" width="300" title="you have me!">

## 功能介绍
Vnet是一个代理工具,在某些网络条件受到限制的情况先提供突破服务.

## 开发计划
- [ x ] shadowsocsk代理协议
- [  ] kcp自定义协议
- [ x ] 代理服务流量统计
- [  ] 代理服务速度监控(正在测试)
- [  ] restful api
- [  ] 服务器cpu 内存 硬盘 上传下载速度监控

## 已知问题
- [ ] log formatter setdepth 多线程问题待改进



## 运行
linux去release页面下载对应的指令集二进制文件给运行权限直接运行,根据提示输入对应的配置好

window直接运行exe

linx:
```
chmod +x server && ./server
```

## 编译方式
```
go get -u -d github.com/rc452860/vnet/...
```

进入$gopath/rc452860/vnet目录

```
go build cmd/server/server.go
```