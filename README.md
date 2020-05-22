### Web--Training v1.0

⭐ 靶场链接为度盘：链接：https://pan.baidu.com/s/1I0oJLdVzjv0grHzlgITvLg 提取码：dcib

>    靶场要点：
>    
>    1. 本靶场为自搭建，素材源码来自互联网以及自编写，若有侵权，联系我删除
>    
>    2. 本靶场只用作Web安全初学者所用，靶场收集来之不易，且用且珍惜
>    
>    3. 本靶场不用做任何商业用途，只作学习交流
>    

  - 靶场系统
     - Window Server 2003 Enterprise Edition Service Pack 2
  - Web服务（由PHPstudy、JSPstudy以及自安装）
     - php 5.3.29/5.3.29-nts/5.2.17
     - Apache 2.4.10
     - Nginx 1.6.2
     - MySQL 5.5.40
     - phpMyAdmin 3.5.8.2
     - OpenSSL 1.0.1e&0.9.8y
     - JDK 1.7_51
     - Tomcat 6.0.44
     - IIS6.0
     - PostgreSQL 8.2
     - SQL Server 2005
     - Redis 2.6.8-pre2
  - 另安装扩展
     - ISAPI_Rewrite3
  - Web Application Firewall     
     - SafeDogIIS（安全狗）V4.0
     - D盾 v2.1.5.4
     - 云锁 v3.1.18.5
     - libinjection-3.10.0（有安装包，暂未安装）
     - ModSecurityIIS_2.9.3-32b.msi（有安装包，暂未安装）
     - SafeDogApache（安全狗）V4.0（有安装包，暂未安装）
     - ngx_lua_waf-0.7.2（有安装包，暂未安装）
     - PHPIDS-0.7（有安装包，暂未安装）

### 靶场

#### SQL注入

  - 源码靶场

端口|靶场|备注
:--:|:--:|:--:
8001|Access注入|
8002|Mssql注入| 
8003|Mysql注入|
8004|Postgresql注入|
8011|Cookie注入|
8012|伪静态注入|需要开启ISAPI_Rewrite3重写扩展
8013|Get注入|
8014|Post注入|
8015|二阶注入|
8016|XFF注入|
8017|XML文件注入|只是文件存储，非XXE
8018|Union联合注入|
8019|报错注入|
8020|Boolean注入|
8021|Base64注入|
8022|时间注入|
8023|宽字节注入(Get)|
8024|堆叠注入|
8025|Insert型注入|
8026|Delete型注入|
8027|Update型注入|
8028|搜索型注入|
8029|宽字节注入|有注入用代码widebytes-post.php/widebytes-post.py
8030|Order by注入|
8031|Group by注入|
8032|二次编码注入|
8033|万能密钥-简单|
8034|万能密钥-Uinon|

  - CMS/比赛靶场

端口|靶场|备注
:--:|:--:|:--:
8051|Bluecms|Http头注入
8052|74cms|二阶注入
8053|Jeany|搜索型注入
8054|南方数据|Cookie注入
8055|Beecms|后台注入
8056|W78cms|搜索框注入
8057|Shop7z|偏移注入
8058|佛山发发鱼|偏移注入
8059|Phpcms_v9|Authkey注入，有注入用代码phpv9 authkey.php
8060|Xycms家庭装修|Access注入
8061|MetInfo v5.0|Sql注入
8062|Xycms搬家|Sql注入
8063|Xdcms|Post注入
8064|19年强网杯随便注|堆叠注入，需初始化数据库


#### XXE

  - 源码靶场

端口|靶场|备注
:--:|:--:|:--:
8101|XXE有回显注入|
8102|XXE无回显有报错注入|
8103|XXE无报错无回显注入|
8104|Simplexml_load_string|php函数
8105|DOMDocument|php函数
8106|SimpleXMLElement|php函数

  - CMS/比赛靶场

端口|靶场|备注
:--:|:--:|:--:
8151|S-CMS医院建站系统v3.0|
8152|MetInfo-v6.0.0|
8153|Phpshe-v1.7|

#### SSRF

  - 源码靶场

端口|靶场|备注
:--:|:--:|:--:
8201|ssrf全测试|多种协议的测试，dict/http/gopher/file等协议，测试时可开启redis-server
8202|ssrf无回显|
8303|ssrf-http(s)测试|有注入用代码301.php/302.php
8204|file-get-contents|php函数
8205|fsockopen|php函数

  - CMS/比赛靶场

端口|靶场|备注
:--:|:--:|:--:
8251|Disccuz-x3.1|


#### 文件上传

  - 源码靶场

端口|靶场|备注
:--:|:--:|:--:
8301|Nginx文件解析漏洞|需开启Nginx
8302|Apache文件解析漏洞|需开启Apache
8303|IIS文件解析漏洞|需开启IIS
8304|Upload靶场的链接与解析|建议玩Upload-labs时边看此端口的内容
8305|表单无按钮提交|
8306|修改上传目录|
8307|双文件上传|
8308|Fckeditor编辑器 v2.4.3|基于Xycms
8309|Fckeditor编辑器 v2.5|基于Xycms
8310|Fckeditor编辑器 v2.6.3|基于Xycms
8311|EWEB编辑器 v5.5|基于Xycms，有注入用代码eweb5.5.html

  - CMS/比赛靶场

端口|靶场|备注
:--:|:--:|:--:
8351|dedecms v5.7 sp1|上传目录修改
8352|南方数据|双文件上传
8353|冠龙科技 v6.0|目录遍历/上传
8354|W78企业建站系统|利用exp构造上传

#### php相关

  - 源码靶场

端口|靶场|备注
:--:|:--:|:--:
8401|php相关测试|文件包含、PHP伪协议、代码执行、变量覆盖、目录遍历、URL重定向
8402|__wakeup()|php反序列化wakeup函数的绕过
8403|php://input|php伪协议
8404|php://filter|php伪协议

  - CMS/比赛靶场

端口|靶场|备注
:--:|:--:|:--:
8451|易库影视CMS|文件包含
8452|海洋CMS v6.28|代码执行
8453|dedecms v5.7|变量覆盖
8454|20年网鼎杯青龙组Areserialize|php反序列化
8455|buuoj极客大挑战2019PHP|php反序列化

#### 集成靶场以及Webshell

端口|靶场|备注
:--:|:--:|:--:
9001|mssql-labs|
9002|sqli-labs|
9003|xxe-lab|
9004|phpaudit-xxe|
9005|xss-labs|
9006|upload-labs|
9051|WEBSHELL箱子管理系统 V1.0|
9052|魔神WebShell

#### 测试

端口|靶场|备注
:--:|:--:|:--:
88|test|Everyone的System权限
89|cgi-test|Everyone的System权限、cgi测试
80|默认网站|防冲突停止使用


### 待补充

#### 大靶场

  - XSS
  - CSRF
  - 逻辑漏洞
  - Getshell靶场
  - JSP相关漏洞测试：Stuct2、Java反序列化漏洞、Tomcat部署漏洞、WebLogic攻击
  - ▲ 各种靶场的更多CMS
  - ▲ 可进行测试的CTF靶场



