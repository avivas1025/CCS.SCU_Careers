## 📌技术学习路线-测试开发岗/测试岗

   可以按照后端开发岗的技术栈（[后端开发岗技术学习路线](./6roadmap/back_end_roadmap.md)）来准备，包括：编程语言、数据库、linux操作系统（常用命令和shell脚本），以及补充一些有关测试的知识，包括，测试体系、测试技术，测试流程。
   
   有关测试知识的部分个人认为可以按照如下学习路线。
   
   <mark>当然从求职的角度而言，作为应届生来说，用人单位的要求并不会太高，所以测开岗位的准备重点还是『八股+算法+项目+测试基础』，进阶和高阶部分需要了解即可（我是实习接触到了自动化，所以面试官也针对这部分有很多提问。）：</mark>
   ![](/6roadmap/test_roadmap.png)
   
#### 1. 编程能力
测试开发的核心是“开发能力”，必须至少掌握一门语言：
 - 在准备算法/刷题，相信已经具备了相当的开发能力。
 - Python（也推荐学习）：语法简单，生态丰富（Pytest、Requests、Selenium等库）。
 - 额外的加分项：Shell脚本（Linux环境操作）、SQL（数据库验证）。


#### 2. 测试基础
- 软件测试理论
   - 测试类型：功能测试、集成测试、系统测试、回归测试、冒烟测试等。
   - 测试方法：黑盒（等价类、边界值、因果图）、白盒（语句覆盖、路径覆盖）、灰盒测试。
   - 测试流程：需求分析→测试计划→用例设计→执行→缺陷管理（Bug生命周期）。
   - 推荐学习资源：《软件测试的艺术》（经典书籍）、ISTQB认证（可选）。

- 测试工具入门（尝试使用测试工具对已有的项目进行测试）
  - 手工测试工具：JIRA（缺陷管理）、Jmeter（压力测试）、 TestLink/Xray（测试用例管理）。
  - 接口测试工具：Postman、Swagger（熟悉HTTP协议、RESTful API）。

#### 3. 自动化测试
- UI自动化
 - Web端：Selenium + Pytest/TestNG + Page Object模式。
 - 移动端：Appium（Android/iOS），结合ADB命令。

- 接口自动化
 - 工具：Requests（Python）、RestAssured（Java）。

- 单元测试
 - 框架：Pytest（Python）、JUnit/TestNG（Java）。
 - 覆盖率：Coverage.py（Python）、Jacoco（Java）。

#### 4. 持续集成与DevOps（进阶）
- CI/CD工具链
  - Jenkins：Pipeline脚本编写、插件配置（集成Git/SonarQube）。
  - GitLab CI/GitHub Actions：自动化触发测试任务。

- 代码质量管理
  - SonarQube：静态代码分析。
  - Allure/ExtentReport：自动化测试报告生成。

#### 5.性能测试（进阶）
 - 工具与场景
   - JMeter：压力测试Web/API，熟悉线程组、断言、监听器。
   - Locust（Python）：分布式压力测试。

 - 监控与分析
  - 服务器监控：Prometheus + Grafana。
  - 性能调优：数据库索引、缓存（Redis）、JVM参数。

#### 6.测试框架开发（高阶）
- 自定义测试框架
  - 设计数据驱动、关键字驱动框架。
  - 封装通用组件（如日志、邮件通知、数据库连接池）。

- 开源贡献
   - 参与开源项目（如Pytest插件开发）。



🔸ps: 网上有很多专业的测试内容，从UI测试、接口测试、性能测试再到整个自动化测试框架的搭建。这部分可以在确定走测试路线后做深入学习。甚至再拿到offer后学习也不会迟。


