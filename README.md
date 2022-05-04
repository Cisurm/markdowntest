# Security： Its Assurance Case
## 安全要求
### 保密
#### 维护用户隐私
	我们的关键要求之一是“保护用户及其隐私”。以下是关于我们如何做到这一点的简短讨论。
首先是用户密码：
	本地帐户的用户密码仅作为迭代的用户信息存储在服务器上，因此无法以未加密的形式检索。
发送到系统的任何用户密码都由应用程序路由发送到用户控制器 的方法调用用户模型 ，非公开数据在静态和动态中都是保密的（特别是用户密码受到保护）。我们的部分隐私要求是“未经用户同意，不得将用户活动暴露给不相关的网站（包括社交媒体网站）”；如下这是我们如何做到的：
其次是站点：
我们必须首先定义不相关站点的含义。“相关”站点是我们直接用来提供服务的站点，特别是我们的云提供商日志/入侵检测服务。实际上，相关站点必须（在各种情况下）接收有关用户的一些信息（至少用户正在尝试做某事时）。这适用于所有网站，因此也适用于我们的网站。
