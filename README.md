<!--
 * @Author: your name
 * @Date: 2019-11-09 23:02:06
 * @LastEditTime: 2019-11-09 23:13:29
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /cms/README.md
 -->
# react全家桶 + ts + koa写的一个博客管理系统和博客展示系统

## FE 用法
> https://mp.weixin.qq.com/s?__biz=MzI1NTE1NjQwNA==&mid=2651695240&idx=1&sn=838f2ba029ee5b571338ce626d2ef659&chksm=f1c34153c6b4c8458b549009e76b6204755f4f825f1a6f2f0e3a3085a983d3745a42f49a4843&mpshare=1&scene=1&srcid=&sharer_sharetime=1573782135026&sharer_shareid=c5180dbda1f8da6adf9971665f649244&key=f8fb043b3d2681a768fcf209a66d2724b0742db134ff445d92c3ad71ebe43d5969336ff4e4e3350f3bd9ccaf697fde6769168c06e7775550333ba0840163710f722a3abd004b21142c45459402749ad6&ascene=1&uin=MTk4MTg1NTgxMQ%3D%3D&devicetype=Windows+10&version=62060834&lang=zh_CN&pass_ticket=pzTA%2FCHFp76AtgRZ22ZbWd1vt2U4nlLD%2FkFGMTQ2xtYlfVLweb26zDNayWRy%2F7U%2B

### 安装
+ npm install

### 使用
+ npm start

## BE 用法
### 安装
+ npm install

### 使用
+ npm run dev

## 数据库
+ blog表：文章

    | 名称        | 类型    |  长度  |  主键 | 
    | --------   | -----:   | :----: | :----: |
    | id        | int      |   11    | true| 
    | title       | varchar      |   255    | false |
    | authore        | varchar      |   255    | false|
    | content        | varchar      |   255    | false|
    | createdAt        | datetime      |   0    | false|
    | updatedAt        | datetime      |   0    | false|

+ comment表：评论

    | 名称        | 类型    |  长度  |  主键 | 
    | --------   | -----:   | :----: | :----: |
    | cid        | int      |   11    | true| 
    | comment       | varchar      |   255    | false |
    | id        | int      |   11    | false|
    | createdAt        | datetime      |   0    | false|
    | updatedAt        | datetime      |   0    | false|

+ user表：用户

    | 名称        | 类型    |  长度  |  主键 | 
    | --------   | -----:   | :----: | :----: |
    | id        | int      |   11    | true| 
    | username       | varchar      |   255    | false |
    | password        | varchar      |   255    | false|
    | createdAt        | datetime      |   0    | false|
    | updatedAt        | datetime      |   0    | false|
