---
description: 淬炼红心小程序文档
---

# 淬炼红心小程序文档

## 

## 小程序实现

### 开发人员

张佳钰

### 开发及运行环境

* 编程语言

  * wxml
  * wxss
  * javascript

* 开发环境

  * 微信开发者工具
  * postman
  * google chrome

* 运行环境

  微信小程序运行在多种平台上：iOS（iPhone/iPad）微信客户端、Android 微信客户端、PC 微信客户端、Mac 微信客户端和用于调试的微信开发者工具。

  各平台脚本执行环境以及用于渲染非原生组件的环境是各不相同的：

  * 在 iOS 上，小程序逻辑层的 javascript 代码运行在 JavaScriptCore 中，视图层是由 WKWebView 来渲染的，环境有 iOS 12、iOS 13 等；
  * 在 Android 上，小程序逻辑层的 javascript 代码运行在 [V8](https://developers.google.com/v8/) 中，视图层是由自研 XWeb 引擎基于 Mobile Chrome 内核来渲染的；
  * 在 开发工具上，小程序逻辑层的 javascript 代码是运行在 [NW.js](https://nwjs.io/) 中，视图层是由 Chromium Webview 来渲染的

### 界面功能

| 界面名称 | 界面功能 | 相关文件夹 |
| :--- | :--- | :--- |
| contact | 创建，存储联系人 | contact |
| demands | 查找需求，展示需求 | demands |
| main | 主页展示 | main |
| makeApply | 需求对接申请管理 | makeApply |
| makeDemand | 需求管理，创建，修改，删除，查找需求 | makeDemand |
| mine | 个人中心，包含我的组织，常用联系人，我的需求，我的对接 | mine |
| myApply | 我申请的对接 | myApply |
| myDemands | 我发布的需求 | myDemands |
| organization | 组织管理 | organization |
| makeApplyOrganition | 加入组织的申请管理 | organization/makeApplyOrganition |
| makeOrganization | 创建组织 | organization/makeOrganization |
| myOrganizations | 我创建和加入的组织 | organization/myOrganizations |
| organization | 组织信息 | organization/organization |
| organizations | 组织搜索以及显示所有组织 | organization/organizations |
| makeUserInfo | 个人信息添加以及修改 | userinfo/makeUserInfo |

### 工具模块

|  |
| :--- |


#### api.js\(接口封装\)

对接口中需要传输的url，传输数据等进行定义

#### formUtil.js\(表单工具\)

检测表单中的空内容并提示给用户端，仅可用于检测表单是否存在空填内容

#### http.js\(http封装\)

将`wx.request`封装，简化调用流程

#### timeUtil.wxs\(时间格式化工具\)

将时间戳转化为格式化时间

#### tool.wxs\(显示格式化工具\)

将距离，地址格式化显示

#### util.js

将获取的经纬度通过接口获取地址详情

### 界面模块

#### 登陆界面



![](.gitbook/assets/image.png)







