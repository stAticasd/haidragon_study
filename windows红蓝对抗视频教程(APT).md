# windows红蓝对抗视频教程(APT)  
* 1.介绍

# 逆向基础
## 工具篇
* 2.X64dbg使用教程一
* 3.X64dbg使用教程二
* 4.X64dbg使用教程三
* 5.X64dbg使用教程四
* 6.X64dbg使用教程五
* 7.X64dbg使用教程六
* 8.X64dbg实战分析 dump 加密函数
* 9.OllyDBG常用操作 
* 10.windbg 
* 11.ida

## 开发基础
### 用户层开发基础
* 12.vc++开发环境搭建(VS)
* 13.编译第一个动态库(DLL)

### PE文件
* 14.认识PE文件(介绍)
* 15.解析PE文件头
* 16.导入导出表
* 17.解析导入导出表
* 18.重定表
* 19.解析重定表
* 20.其它表解析

### 驱动开发基础
* 21.驱动开发环境搭建 
* 22.驱动基本原理 
* 23.驱动层与用户层通信 
* 24.驱动中的相关函数

### 注入与hook
#### 用户层
* 25.hook原理
* 26.windows消息hook 
* 27.内联(inline)hook
* 28.64位内联hook
* 29.IAT hook
* 30.注入原理 
* 31.远程线程注入 
* 32.IAT注入 
* 33.APC式注入 
* 34.反射式注入

#### 驱动层
* 35.驱动层--IRP hook
* 36.驱动层--Object hook
* 37.驱动层--SSDT hook
* 38.驱动层--SSSDT hook 
* 39.驱动层--VT hook
* 40.驱动层--远程线程注入 
* 41.驱动层--APC注入 
* 42.驱动层--IAT注入 
* 43.驱动层--全局内存注入

### 常用注入与hook工具
* 44.frida介绍
* 45.frida常用命令
* 46.利用frida 遍历模块
* 47.利用frida 遍历导入导出表
* 48.利用frida hook 导出函数
* 49.利用frida hook 未导函数
* 50.利用frida 实战分析 Proxifier

# 红队基础 

## 介绍(了解黑客如何攻击)
* 51.红队介绍

## Active Directory与Kerberos滥用
* 52.从域管理员到企业管理员
* 53.Kerberoasting
* 54.Kerberos协议---Golden Tickets
* 55.Kerberos协议---Silver Tickets
* 56.AS-REP Roasting
* 57.Kerberoasting(RC4) 
* 58.Kerberos无约束委派
* 59.Kerberos约束委派(KCD)
* 60.计算机对象接管
* 61.域破坏(DC Print Server Kerberos)
* 62.DCShadow 
* 63.从域控制器dump哈希
* 64.Active Directory枚举
* 65.滥用AD ACL / ACE
* 66.特权帐户和令牌特权
* 67.从DnsAdmins到SYSTEM到域破坏
* 68.Pass the Hash(Machine$ Accounts)
* 69.BloodHound(kali)
* 70.adminsdholder利用(权限维持)
* 71.AD枚举(无RSAT或管理员权限)
* 72.使用dsacls枚举AD对象权限
* 73.AD密码Spraying

## 红队基础设施
* 74.http转发中继
* 75.smtp转发中继
* 76.使用Modlishka钓鱼
* 77.使用Terraform钓鱼
* 78.使用CobaltStrike钓鱼
* 79.使用Powershell
* 80.Spiderfoot 

## 初始访问(Initial Access)
* 81.网页植入恶意代码(水坑式钓鱼)
* 82.利用常用软件植入后门(PE文件 案例phpstudy)
* 83.利用常用文件植入后门(漏洞利用 案例office文档)
* 84.图片植入后门
* 85.PDF文件植入后门
* 86.利用邮件植入后门(鱼叉式钓鱼)

## 代码执行(Execution)
* 87.利用regsvr32绕过白名单
* 88.利用mshta绕过白名单
* 89.利用rundll32.exe绕过白名单
* 90.控制面板项执行原理
* 91.控制面板项执行dll
* 92.利用CMSTP绕过白名单
* 92.利用InstallUtil绕过白名单
* 94.利用MSBuild绕过白名单
* 95.利用Forfiles绕过白名单
* 96.利用WMIC绕过白名单
* 97.远程动态数交换
* 98.命令行界面 
* 99.利用签名脚本代理执行
* 100.利用chm绕过白名单
* 101.利用IEExec绕过白名单
* 102.利用MSIexec绕过白名单
* 103.利用Pcalua绕过白名单
* 104.利用Regsvcs/Regasm绕过白名单
* 105.利用Scripting脚本绕过白名单
* 106.利用Trusted Developer Utilities 
* 107.利用SyncAppvPublishingServer
* 108.利用Winword绕过白名单
* 109.利用XSL Script Processing
* 110.利用本地任务调度
* 111.利用计划任务
* 112.利用用户图形化界面
* 113.利用DCOM
* 114.利用Powershell
* 115.利用SMBexec
* 116.利用WinRM
* 117.利用Language LUA
* 118.利用INF-CST
* 119.Reflection.Assembly
* 120.msconfig
* 121.利用DXCap.exe
* 122.利用sigverif.exe
* 123.利用Register-cimprovider.exe
* 124.利用xls mimikatz

## 高级注入加代码执行
* 125.从PE资源文件中加载Shellcode
* 126.Process Hollowing 
* 127.NtCreateSection/NtMapViewOfSection注入
* 128.注入.NET Assembly到非托管进程
* 129.Mapping Injection
* 130.InjectFromMemory
* 131.通过tls注入
* 132.PE加载器实现

## 持久化（Persistence）
* 133.Office -SVG
* 134.ADS 数据流
* 135.RunOnceEx
* 136.winlogon_regedit
* 137.ImageFileExecutionOptions
* 138.内存加载执行mimikatz(dll劫持)
* 139.Run-key-hexacorn持久性
* 140.利用各种注册表项实现权限维持
* 141.映像劫持（IFEO）
* 142.COM劫持
* 143.CLR(Common Language Runtime)
* 144.CAccPropServicesClass＆MMDeviceEnumerato
* 145.劫持MruPidlList
* 146.WMI
* 147.Waitfor.exe
* 148.bitsadmin
* 149.DoubleAgent
* 150.Office-Persistence
* 151.ALPC
* 152.DLL劫持
* 153.利用计划任务权限维持
* 154.利用服务权限维持
* 155.利用Sticky权限维持
* 156.AddMonitor()
* 157.netsh helper
* 158.劫持默认扩展名
* 159.修改.lnk快捷方式
* 160.利用屏保程序权限维持

## 防御规避(免杀 Defense Evasion)


## 基础信息收集(Enumeration and Discovery)
## 权限提升

## 凭证访问和转储(Credential Access & Dumping)
## 横向移动
## 命令控制(C2/C&C) 远控
## 信息窃取(Exfiltration) 
## 高级自动化工具
* burp suite
* Cobalt Strik
* Metasploit Framework

# 蓝队基础 

## 介绍(了解白帽如何防御)
## yara 
## 流量
## 行为
## 工具


# apt 教程
* apt 介绍

* 各种方向的样本分析 

sysmon 监听日志

