# PartyMemberStudy
高校党建学习小程序 智慧建党学习小程序 角色：普通用户、党校学员、系统管理员、校党委管理员、二级分党委管理员； 亮点：自动组题、协同过滤算法、Echarts图形化分析；
所有源码均本人开发，项目是前后端分离的，所有的项目都具备了完整的业务逻辑，不仅仅局限于基础的增删改查（CRUD）操作，系统亮点众多。

本文注重于计算机毕业设计选题指导，列出题目均有源码， 大家可以去【公众号】(毕业终点站)获取或者加我【qq】(2112698948)提意见(别忘记Star哟)。备注：git

声明：仅用于学习使用，请勿用于任何商业行为！

1.系统非商用，非开源，非无偿。

2.由本人开发，如需源码，请联系以下方式，qq:2112698948。

3.项目有很多，并未全部上传，如果未找到想要的，可直接咨询。
<font style="color:#117cee;">🎈</font><font style="color:#117cee;">系统亮点：自动组题、协同过滤算法、Echarts图形化分析；</font>

# <font style="color:#48b378;">一.系统开发工具与环境搭建</font>
## <font style="color:#262626;">1.系统设计开发工具</font>
<font style="color:#262626;">后端使用Java编程语言的Spring boot框架</font>  
<font style="color:#262626;">项目架构：B/S架构</font>  
<font style="color:#262626;">运行环境：win10/win11、jdk17</font>



<font style="color:#48b378;">小程序：</font>

<font style="color:#262626;">技术：Uniapp；UI库：ColorUI； </font>

<font style="color:#262626;">开发工具：HBuilderX；</font>

---

<font style="color:#48b378;">前端：</font>  
<font style="color:#262626;">技术：框架Vue3 ；UI库：Element-Plus；</font>  
<font style="color:#262626;">开发工具：Visual Studio Code；</font>

---

<font style="color:#48b378;">后端:</font>  
<font style="color:#262626;">技术：Java语言、mybatis-plus、Spring boot框架；</font>  
<font style="color:#262626;">开发工具：IDEA 2025版本；</font>

---

<font style="color:#48b378;">数据库：</font>  
<font style="color:#262626;">数据库：mysql5.7/8.0 </font>  
<font style="color:#262626;">数据库工具：Navicat12版本；</font>

---

# <font style="color:#48b378;">二.系统实现（部分截图）</font>
  高校党建学习小程序共有五个角色，分别是<font style="color:#DF2A3F;">普通用户、党校学员、系统管理员、校党委管理员、二级分党委管理员</font>。前台面向<font style="color:#DF2A3F;">普通用户</font>和<font style="color:#DF2A3F;">党校学员</font>，提供党建资讯浏览、在线课程学习、学习资料查看与收藏、线下培训报名/记录、消息通知、测评中心中的题型练习、随机练习、模拟考试、考试记录、题目收藏、错题本，以及个人信息、密码修改、微信绑定、入党申请和荣誉证书等功能；后台角色包括<font style="color:#DF2A3F;">系统管理员、校党委管理员、二级分党委管理员</font>，其中系统管理员主要管理账号和院系，校党委管理员负责文章、课程、学习资料、题库、试卷考试及答题记录等内容和考试管理，二级分党委管理员负责入党申请审核、党员学员管理、线下培训管理以及院系学员和线下培训统计；代码中还体现了入党申请审核通过后会把申请人角色变更为党校学员，并发送消息通知。  

## <font style="color:#222222;">业务流程</font>
**<font style="color:#222222;">课程建设流程</font>**<font style="color:#222222;">：后台先维护课程分类、课程内容和课程步骤，同时补充学习资料，形成党员学习资源库。</font>

**<font style="color:#222222;">学习流程</font>**<font style="color:#222222;">：学生在小程序中浏览课程详情并逐步完成学习内容，系统持续沉淀课程学习进度和学习记录。</font>

**<font style="color:#222222;">练习测试流程</font>**<font style="color:#222222;">：学生进入测试中心或随机练习页面完成答题，系统记录作答结果、错题数据和答题日志。</font>

**<font style="color:#222222;">问卷与申请流程</font>**<font style="color:#222222;">：平台可发布问卷供学生填写，学生也可以在线提交入党申请，后台统一查看结果和申请状态。</font>

**<font style="color:#222222;">活动参与流程</font>**<font style="color:#222222;">：学生浏览活动详情并参与活动互动，系统记录活动参与和评论数据。</font>

**<font style="color:#222222;">核心业务闭环</font>**<font style="color:#222222;">：平台围绕“课程建设 - 学习进度 - 练习测试 - 错题沉淀 - 活动参与 - 入党申请与学习统计”形成党员学习闭环。</font>

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970828594-a85d146b-bdd9-4367-b087-2716eae07c67.png)

## 2.1 普通用户
### 2.1.1 首页
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970827792-734e936a-6335-46f9-84c6-7f71ed4363a8.png)

### 2.1.2 线下培训
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970828608-abbc3f0b-2004-4c34-a933-adad6d4aa861.png)

### 2.1.3 课程列表
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970827462-d176f9a4-bbc6-4c18-86c3-fa5f9882f731.png)

### 2.1.4 资讯列表
相关推荐为协同过滤算法推荐。

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970828082-b1aa7202-717f-42b8-be6e-56114c9bdd4d.png)

### 2.1.5 学习资料学习
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970828466-a38776f3-f2fb-4ce4-af69-9b727c1e163d.png)

### 2.1.6 题型练习
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970828716-4c3f347b-3c96-4505-8d28-f2a7ceefe6a1.png)

### 2.1.7 考试
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970829156-acd0ce37-6c5c-4a89-9401-adec00ab02b5.png)

### 2.1.8 考试答题结果
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970829375-c44bea14-2dfc-4fda-a599-b92d482b120f.png)

### 2.1.9 练习/错题本
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970830519-a19661d1-7ad7-467a-a2dc-aabbe144e5c1.png)

### 2.1.10 个人中心
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970830029-7336cec7-8e3b-49d2-8067-2f90e213ee35.png)

## 2.2 党校学员
普通用户进行入党申请后成为党校学员。

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970830396-12caabf5-9caf-413c-b743-f21af1417797.png)

## 2.3校党委管理员
### 2.3.1 文章管理
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970832883-2b6776a0-9426-4549-b597-884d5a61370e.png)

### 2.3.2 文章统计
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970831901-b4d7d6d3-2604-4075-9b37-4f16d1f22ede.png)

### 2.3.3 课程列表
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970833959-2fa6f1bf-a8e9-4bb7-bd4a-5244f4c7fe15.png)

### 2.3.4 学习资料
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970834677-001f1414-5833-4759-ba14-249b4cf13f77.png)

### 2.3.5 题库管理
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970836825-619bd634-4175-4c6f-bed1-6478a69f7672.png)

### 2.3.6 考试列表
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970837068-e6a0cd6d-3e83-4304-ad85-bd82a2ebbddc.png)

### 2.3.7 组题
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970838541-02ae6410-2777-4838-a124-6b8b83eca03f.png)

### 2.3.8 用户答题
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970838276-ccc7b13d-54f6-41c3-8fe4-78196d7727c1.png)

## 2.4 二级分党委管理员
### 2.4.1 入党审核
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970838226-006f4143-bb6f-4d11-aa3a-e47559809075.png)

### 2.4.2 党员学员
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970838158-cab3e672-c2ef-4995-9961-c3d9aba6c36b.png)

### 2.4.3 线下培训列表
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970838401-72181cef-0451-4842-a25f-a2f188da54bf.png)

### 2.4.4 线下培训列表
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970838902-beb12881-032b-410c-9f09-2649a786218a.png)

### 2.4.5 院系学员统计
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970839148-d9372140-2d5d-4253-a115-46a3e6f3a3bf.png)

### 2.4.6 线下培训统计
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970839195-27e261c2-3012-44aa-9ebb-fa671f41bfcf.png)

## 2.5 系统管理员
### 2.5.1 账号管理
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970839390-75ffcee8-4e74-4502-9242-b788a07dba2f.png)

### 2.5.2 院系列表
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970839469-ca9b4cff-77b9-4cb3-8a3d-373a1ff2b603.png)

# <font style="color:#48b378;">三.系统代码结构截图</font>
## <font style="color:#262626;">3.1 前端</font>
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970840165-c3c0d728-ea0e-49b7-ac41-b09621a74e7e.png)

## 3.2后端
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970840152-728055c7-72af-4e7b-aa77-285e046dde3a.png)

## 3.3 小程序
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970840718-c747a1b1-844c-4e53-8ae0-65a6cb71572c.png)

## 3.4 数据库
34张表

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/45326128/1784970839953-0f21228a-3dad-4f90-a634-7eb6e408bd17.png)

# <font style="color:#48b378;">四.</font><font style="color:#1aad19;">源码获取</font>
<font style="color:#000000;">1.原创系统非商用，非开源，非无偿。</font>

<font style="color:#000000;">2.项目有很多，并未全部上传，如果未找到想要的，可直接咨询。</font>

