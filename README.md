# 医患档案管理系统

## 前言

医患档案管理系统是一款针对医疗行业中医生与患者之间的信息管理需求而开发的实战项目。该系统基于Java语言和MySQL数据库，采用Spring Boot框架和Vue前端技术进行开发。本文将为您详细介绍该项目的相关内容，包括技术选型、核心代码以及如何获取免费源码等。

## 内容介绍

本项目主要实现了以下功能：

1. 医生和患者的基本信息管理：包括医生的专业、职称、出诊时间等，患者的个人信息、病历信息等。
2. 预约挂号：患者可以根据医生的专业和出诊时间进行在线预约挂号。
3. 档案查询：医生和患者可以查询各自的档案信息，便于跟踪病情和治疗效果。
4. 消息通知：系统可以实时推送预约成功、取消预约等通知，方便医患双方及时了解预约状态。

## 技术介绍

- 语言：Java
- 使用框架：Spring Boot
- 前端技术：JS、Vue、css3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

## 核心代码

以下是项目中的一部分核心代码，展示了医生信息管理的接口：

```java
@RestController
@RequestMapping("/api/doctor")
public class DoctorController {

    @Autowired
    private DoctorService doctorService;

    // 获取医生列表
    @GetMapping("/list")
    public ResponseEntity<List<Doctor>> getDoctorList() {
        List<Doctor> doctors = doctorService.list();
        return ResponseEntity.ok(doctors);
    }

    // 添加医生
    @PostMapping("/add")
    public ResponseEntity<String> addDoctor(@RequestBody Doctor doctor) {
        doctorService.add(doctor);
        return ResponseEntity.ok("添加成功");
    }

    // 更新医生信息
    @PostMapping("/update")
    public ResponseEntity<String> updateDoctor(@RequestBody Doctor doctor) {
        doctorService.update(doctor);
        return ResponseEntity.ok("更新成功");
    }

    // 删除医生
    @PostMapping("/delete/{id}")
    public ResponseEntity<String> deleteDoctor(@PathVariable("id") int id) {
        doctorService.delete(id);
        return ResponseEntity.ok("删除成功");
    }
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img11.360buyimg.com/ddimg/jfs/t1/311257/38/26957/87051/689ee95dF855ca6b4/cc8cc2d797777c92.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/326099/34/4781/15180/689ee934F3b3eb185/14888607f1268d5c.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/324460/40/4829/23030/689ee935F05e496fa/bd7077f1a8d829a8.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/322540/15/11118/14452/689ee935F703272b0/af4dc62a791a0644.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
