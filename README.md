
## **2.线上预约陪诊系统（Java，JS，micro-service，Vue）**
微服务应用课程设计
###  2.1 简介
一个线上预约陪诊系统，用户可通过H5小程序预约陪诊员上面进行陪诊服务。后端服务器使用Java开发，前端基于Vue开发面向用户的H5应用及面向管理员的后台系统。
###  2.2 技术细节
- 语言及框架/工具：
    - Java，JavaScript
    - SpringCloud，MyBatis，OpenFeign，Vue，MySQL，JWT
    - Nacos，SpringCloud GateWay，Docker
- 服务器：
    - 根据不同的业务场景，将系统划分成订单管理，用户中心等不同微服务，使用Docker部署各服务。
    - 使用Nacos作服务注册与配置中心，使用SpringCloud Gateway作网关，不同服务间使用OpenFeign通信。
    - 使用MySQL存储订单，用户，陪诊员等数据。
    - 使用开源工具[renren-generator](https://gitee.com/renrenio/renren-generator)通过数据库结构快速生成订单，用户等数据查询接口模板代码，加快开发速度。
- 客户端/后台管理系统：
    - H5应用基于开源商城项目[众邦科技/CRMEB-H5](https://gitee.com/ZhongBangKeJi/CRMEB-H5)。根据陪诊服务场景对开源项目代码进行删减，修改，重构以实现对应的业务逻辑。
    - 后台管理系统使用开源工具[renren-fast-vue](https://gitee.com/renrenio/renren-fast-vue)快速构建。

###  2.3 功能演示
- 系统架构：<br>
![系统架构图][pic-2.3.0]<br>
- 客户端截图：<br>
![客户端截图][pic-2.3.1]<br>
- 后台管理系统：<br>
![后台管理系统截图][pic-2.3.2]<br>
- nacos配置：<br>
![nacos配置中心截图][pic-2.3.3]<br>
![nacos注册中心截图][pic-2.3.4]<br>

###  2.4 项目仓库
- 服务器：<br>
<https://github.com/HaoyuanMa/micro-service-server>
- 客户端：<br>
<https://github.com/HaoyuanMa/micro-service-front>
- 后台管理系统：<br>
<https://github.com/HaoyuanMa/micro-service-admin>

---


[pic-2.3.0]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/6a53e09c-d00a-4165-ac13-bfdd5d56df70.png
[pic-2.3.1]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/b4706df5-f348-49bd-a7e3-f24368b8a185.png
[pic-2.3.2]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/901482dd-2bd4-4dac-a14a-457902558a6c.png
[pic-2.3.3]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/a861fc72-36a1-4853-b193-d664601138ef.png
[pic-2.3.4]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/dd9802ea-dbdf-48a2-abde-b16841b6685d.png
