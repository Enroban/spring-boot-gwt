# Spring Boot GWT

这个是源自一个大神搭好的框架，使用的Springboot配合GWT，实际上通信方式是JSON。

## 架构

![arch](docs/architecture.jpg)

## TRY

如果想测试可以先到测试地址试试效果[测试地址](https://spring-boot-gwt.herokuapp.com/)

## 开发

需要安装gradle，在本地开发的时候，springboot和gwt需要分别启动。我使用的是idea，在开发的时候，需要为子项目增加JavaWeb框架，并配置web框架的根目录为 [`static/resource`](src/main/resources/static)，否则，gwt会找不到文件

## 打包

``` shell
gradle build
```

之后找到 `build/libs/spring-boot-gwt-1.0.0.jar`，执行下面的命令

```shell
java -jar spring-boot-gwt-1.0.0.jar
```

访问<localhost:8080>就能看到效果了