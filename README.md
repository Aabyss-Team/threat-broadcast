# 渊龙Sec安全团队-威胁情报播报【魔改】

**本项目公开在线地址：[https://threat.aabyss.cn/](https://threat.aabyss.cn/)**
------


## 1# 项目介绍

因为之前看到过在线爬取并自动更新威胁情报的项目，但好多都已经不运营了，我们团队于是便想自己整一个，就有了本项目。

如果你觉得本项目对你有用，欢迎点个Star，感谢各位师傅的关注和支持~

**本项目公开在线地址：[https://threat.aabyss.cn/](https://threat.aabyss.cn/)**

从以下公开的威胁情报来源爬取并整合最新信息：

- 360：https://cert.360.cn/warning
- 奇安信：https://ti.qianxin.com/advisory/
- 红后：https://redqueen.tj-un.com/IntelHome.html
- 绿盟：http://www.nsfocus.net/index.php
- 斗象：https://vas.riskivy.com/vuln
- NVD：https://nvd.nist.gov/feeds/xml/cve/misc/nvd-rss-analyzed.xml
- CNNVD：http://www.cnnvd.org.cn/web/vulnerability/querylist.tag
- Tenable (Nessus)：https://www.tenable.com/cve/feeds?sort=newest
- ~~安全客：https://www.anquanke.com/vul~~ （该平台已经不做 CVE 分析了）
- ~~CNVD：https://www.cnvd.org.cn/flaw/list~~ （该平台不断升级反爬机制，表示尊重）

<details>
<summary><b>关于 CVE 收录的完整性问题说明</b></summary>
<br/>


本程序只收录国内外安全厂商已收录并分析的 CVE，并不收录所有 CVE，需要全量 CVE 的同学可自行去以下站点下载：

- CVEs 官网： https://cve.mitre.org/
- GitHub（CVEs 实时同步）： https://github.com/CVEProject/cvelist
- CIRCL（CVEs 实时同步）： https://cve.circl.lu/ 或 https://cve.circl.lu/api/browse
- 每日 CVE： https://cassandra.cerias.purdue.edu/CVE_changes/today.html

</details>

爬取到的 CVE 情报会作如下处理：

- 【页面播报】 最新的 TOP30 威胁情报会更新到 [Github Page](https://threat.aabyss.cn/)
- 【情报归档】 所有威胁情报会归档到 [sqlite](data/cves.db)




## 2# 目录说明

```
threat-broadcast
├── README.md ............................... [项目说明]
├── main.py ................................. [程序运行入口]
├── cache ................................... [威胁情报缓存]
├── data
│   └── cves.db ............................. [sqlite: 威胁情报归档]
├── docs .................................... [Github Page 威胁情报总览]
├── src ..................................... [项目源码]
├── script .................................. [数据库脚本]
├── tpl ..................................... [模板文件]
├── imgs .................................... [项目图片]
└── logs .................................... [项目日志]
```


## 3# 版权声明

[![Copyright (C) EXP,2016](https://img.shields.io/badge/Copyright%20(C)-EXP%202016-blue.svg)](http://exp-blog.com)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

本项目Fork并参考了 [Mr-xn/threat-broadcast](https://github.com/Mr-xn/threat-broadcast) 和 [EXP-Tools/threat-broadcast](https://github.com/EXP-Tools/threat-broadcast) ，由衷感谢这两个项目~


## 4# 感谢各位师傅🙏

## Stargazers

[![Stargazers repo roster for @Aabyss-Team/threat-broadcast](https://reporoster.com/stars/Aabyss-Team/threat-broadcast)](https://github.com/Aabyss-Team/threat-broadcast/stargazers)


## Forkers

[![Forkers repo roster for @Aabyss-Team/threat-broadcast](https://reporoster.com/forks/Aabyss-Team/threat-broadcast)](https://github.com/Aabyss-Team/threat-broadcast/network/members)


## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Aabyss-Team/threat-broadcast&type=Date)](https://star-history.com/#Aabyss-Team/threat-broadcast&Date)

