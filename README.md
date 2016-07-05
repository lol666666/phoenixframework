# phoenixframework<br>
   phoenixframework是一个自动化测试平台，集代码托管，
 分机（node节点）管理，定时任务，<br>
分布式或并发等方式执行通过phoenix_develop模块调试好的用例。<br>
平台使用SSH4开发，覆盖了webgui，接口，移动mobile等终端的测试与监控。<br>
目前webGUI模块已经完成，兼容chrome，Firefox，IE，httpunit以及phantomjs驱动。<br>
平台原生支持对svn，socket，ftpserver服务器的操作。<br>
平台通过phoenix_develop模块在客户端开发及调试代码，<br>
然后通过将代码托管到phoenix_web控制端，<br>
控制端通过指派多个phoenix_node端方式执行测试用例。
通过使用phoenix_develop开发用例代码的示例，<br>
用例如果在本地调试时没有问题，那么就可以放到控制端进行执行了。<br>
平台网站：http://www.cewan.la 或 http://www.phoenixframe.org<br>
环境搭建及使用说明书：http://my.oschina.net/u/2391658/blog/706055<br>
搜索：测完啦或phoenixframe会有更多关于平台的示例<br>
<br>
最新版本：1.4.8<br>
phoenix_node:优化性能测试时，监控机的CPU及内存数据等的可读性<br>
phoenix_web:增加了ehcache缓存<br>
phoenix_web:增加数据库连接池查看<br>
phoenix_webdriver:commandExecutor方法bug修复<br>
phoenix_webdriver:检查点bug修复<br>
phoenix_web:定时任务细节bug修复<br>
phoenix_webdriver:增加js执行的驱动，再也无需手动强转<br>
phoenix_web:修复接口测试结果统计bug<br>
phoenix_web:个别页面的js重构<br>
phoenix_node:性能测试相关模版细节bug修复<br>
phoenix_web:多个地方增加删除确认提示<br>
phoenix_web:日志增加批量管理方法<br>
phoenix_webdriver:selenide更新到最新3.6,selenium更新到2.48稳定版（兼容safari），selendroid更新到最新0.17<br>
phoenix_webdriver:支持<a href="https://ftp.mozilla.org/pub/firefox/releases/41.0/win32/zh-CN/" target="_blank" title="点击下载Firefox41版本,如打不开，可多试几次">Firefox41</a> /chrome51/IE10/IE11/IE Edge/Safari版本。IE驱动更新到2.53，chrome驱动更新到2.21<br>

<br>
上一版本：1.4.7<br>	
1、修复多个反人类的唯一性约束<br>
2、phoenix_node:jmeter性能测试增加对body参数的支持<br>
3、对平台的各模块代码进行了部分重构，重构后的效果是插件可配置<br>
4、在phoenix_web端增加查看node详细信息的入口<br>
5、phoenix_interface增加对https地址的支持<br>
6、phoenix_develop中增加了一个自己写的并发测试工具<br>
7、抽离出了公共的phoenix_common模块<br>
8、重构了平台项目组织架构，使导入调试等更方便<br>
<br>
系统名称：自动化测试平台<br> 
系统介绍： <br>
【支持的部署方式】：J2EE，Jenkins，maven，J2SE，分布式部署，Jetty部署 <br>
【技术说明】：Apache quartz，Webmagic，httpunit，selendroid，<br>
selenide，Spring+SpringMVC+Hibernate4+Shiro，Executor，Forkjoin，Maven项目管理，<br>
Bootstrap，JQuery，JDK动态编译+反射+执行，DWR，highchat <br>
【权限管理】：方法级别的权限控制 <br>
【覆盖系统类型】：WEB GUI自动化测试，接口自动化测试，Android/IOS app自动化测试，<br>
WEB GUI自动化监控，接口自动化监控，数据库测试，简单安全性测试 <br>
【消息通知】：Email异步发送，短信异步发送，在线日志检视，统计报表生成<br>
【模块介绍】<br>
phoenix_develop：用例代码开发模块<br>
phoenix_node：分布式执行node节点<br>
phoenix_web：平台控制端<br>
phoenix_webdriver：webGUI自动化测试模块<br>
phoenix_mobiledriver：移动设备测试模块<br>
phoenix_interface：接口测试系统<br>
phoenix_db:数据库操作模块，对hibernate4的封装<br>	
phoenix_ftpclient：ftp服务器操作<br>
phoenix_svnclient：对svn进行操作<br>
phoenix_telentclient：对socket服务器进行操作<br>
phoenix_imgreader：验证码及图片的识别模块<br>
phoenix_browser：phoenix定制浏览器，用于属性录制<br>
phoenix_recorder：用于对执行过程录制回放<br>
phoenix_tcpserver：可独立部署在Windows和Linux，用于特殊场景下的操作。如生成或执行shell	<br>
phoenix_jbehave：行为驱动支持	<br>
phoenix_jmeter：基于jmeter定制的专门用于web系统性能测试的模块<br>
