## 前言

岳阳市美术馆预约平台小程序是一个基于Spring Boot的在线预约系统。该系统旨在为用户提供便捷的美术馆参观预约服务，通过微信小程序实现用户与美术馆之间的互动。以下是关于本项目的详细介绍。

## 内容介绍

本项目主要包括以下几个功能模块：用户模块、预约模块、美术馆信息模块、管理员模块。用户模块提供用户注册、登录、个人信息管理等功能；预约模块实现用户在线预约、查看预约记录等功能；美术馆信息模块展示美术馆的基本信息、展览信息等；管理员模块负责审核预约、管理美术馆信息等。

## 技术介绍

本项目采用以下技术栈：

- **语言：Java**
- **使用框架：Spring、Spring MVC、MyBatis、微信小程序**
- **前端技术：JS、Vue、CSS3、Uniapp**
- **开发工具：IDEA/Eclipse，Uniapp**
- **数据库：MySQL 5.7/8.0**
- **数据库管理工具：phpstudy/Navicat**
- **JDK版本：jdk1.8**
- **Maven：apache-maven 3.8.1-bin**
- **前端环境：Node.Js 12、14、16**

## 核心代码

以下是本项目中的一个核心代码片段，展示了如何使用Spring Boot与MyBatis实现用户登录功能。

```java
// UserController.java
@RestController
@RequestMapping("/user")
public class UserController {

    @Autowired
    private UserService userService;

    @PostMapping("/login")
    public ResponseEntity<User> login(@RequestBody User user) {
        User loginUser = userService.login(user);
        if (loginUser != null) {
            return ResponseEntity.ok(loginUser);
        } else {
            return ResponseEntity.status(HttpStatus.BAD_REQUEST).build();
        }
    }
}
```

```xml
<!-- UserMapper.xml -->
<mapper namespace="com.example.mapper.UserMapper">
    <select id="login" resultType="com.example.entity.User">
        SELECT * FROM user WHERE username = #{username} AND password = #{password}
    </select>
</mapper>
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
![封面图片](https://img13.360buyimg.com/ddimg/jfs/t1/344785/12/2855/126135/68c63af1F79d46281/748a10da0221ac0d.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/340228/24/10626/32757/68c63ac8Fc439c32c/77e8e862906feca1.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/349175/19/2805/45655/68c63ac8Fb795f46d/f099c65ff08a0bbb.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/347094/35/3000/26194/68c63ac9F1c2bf8a7/e231231dadd668b0.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/333111/39/13040/22612/68c63ac9Fecd17dd8/799cfe7de80c883c.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/334489/37/12971/54434/68c63ac9Fbac7a594/0b0e5c72422e4991.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/337815/8/9713/66047/68c63acaF7ab0e5e7/3a1ff0acc1d15263.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/342150/11/3163/59337/68c63acaFff641086/13c63ff46f464061.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/348472/22/3200/69776/68c63acaFc3533a57/417941a060a70318.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/329693/12/12931/77718/68c63acaFf6c93932/c67ace617cbb0b0f.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
