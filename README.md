## 前言

大家好，今天我要分享的项目是一个无中介租房系统，基于SSM（Spring、SpringMVC、MyBatis）框架开发。在这个项目中，我们使用了Java作为主要开发语言，并整合了微信小程序、前端技术（JS、Vue、CSS3、Uniapp）等，旨在为广大用户提供一个便捷、高效的租房体验。

## 内容介绍

本项目主要包括以下功能模块：房源展示、房源搜索、房源发布、用户注册登录、在线留言等。通过使用SSM框架和前端技术，实现了前后端分离，提升了系统的可维护性和可扩展性。此外，项目还使用了MySQL数据库进行数据存储，确保数据的安全性和稳定性。

## 技术介绍

- 语言：Java
- 使用框架：Spring、SpringMVC、MyBatis，微信小程序
- 前端技术：JS、Vue、CSS3，Uniapp
- 开发工具：IDEA/Eclipse，Uniapp
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是项目中的一部分核心代码，用于展示房源列表：

```java
// 房源查询接口
@RequestMapping("/list")
public String list(@RequestParam(value = "page", defaultValue = "1") int page,
                  @RequestParam(value = "size", defaultValue = "10") int size,
                  Model model) {
    PageHelper.startPage(page, size);
    List<House> houses = houseService.findAll();
    PageInfo pageInfo = new PageInfo(houses);
    model.addAttribute("pageInfo", pageInfo);
    return "houseList";
}
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
![封面图片](https://img10.360buyimg.com/ddimg/jfs/t1/323962/26/19724/237256/68c57144F33444630/f666bcad7dcb7e9d.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/344901/26/2238/49540/68c5711cF43752ab2/46cf80239fb70693.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/343780/21/2881/39968/68c5711cFd4ac127a/eb28762ec628855c.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/348962/26/2438/17444/68c5711cFb7cd7801/32b5c17b7a681b07.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/324613/23/19622/23142/68c5711cF5e32179c/f3044e8c5dc0bd5a.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/329731/7/12833/21674/68c5711cF7715957a/ad94506ee53fd029.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/332856/3/12639/49325/68c5711cF90b6a211/5c6a7f27766baf77.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/340507/36/10366/48831/68c5711dF867bb4f6/66f23908030f91f7.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/349636/5/2978/55123/68c5711dF4c5debf0/a1e84486360bd941.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/342782/25/2996/223067/68c5711dFb29f9165/a27666ff8c69d334.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
