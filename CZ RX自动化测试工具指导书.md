# CZ RX自动化测试工具指导书
## 1.环境安装
* LabVIEW2018安装包/安装指导 
* NIVISA19.0安装包  
SVN下载路径：https://192.168.18.151/TR8660-CZ001/10测试doc/测试工具/LabVIEW自动化/环境安装
## 2.LabVIEW平台架构
* 架构介绍与学习  
SVN下载路径：https://192.168.18.151/TR8660-CZ001/10测试doc/测试工具/LabVIEW自动化/平台架构学习
## 3.环境搭建
* 将测试工程RFC_tool和Transa Automation文件夹COPY到E盘根目录下  
SVN下载路径：https://192.168.18.151/TR8660-CZ001/10测试doc/测试工具/LabVIEW自动化/测试工程文件
## 4.操作步骤
* 打开RFC_tool文件夹中的串口工具配置串口  
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/Serail%20tool%20FrontPanel%20config.png)
* 根据测试用例仔细配置测试场景(测试输入条件).csv文件
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/RX%20Testcase%20cofig.png)
* 根据测试用例配置对应的调用.xls文件
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/sweep%20file%20list.png)
* 打开Transa Automation文件夹下测试平台主界面vi  
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/Open%20Main%20Project.png)
* 测试平台主界面配置
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/Transa%20Executive%20Fontpanel.png)  
（1）Instrument:  配置SA/SG/VNA IP地址与名称(N9030A/N5182B/SMBV100A/E5071C).  
（2）Test Info:  用户可以自行配置ChipName/Version/TestEngineer等信息,这些信息将会show在测试报告中.  
（3）Moudules:  适用于多用例多场景连跑，点击RunModules,顺序(从上到下)运行用户所有勾选的测试用例以及每条测试用例下所有的测试场景subVi,并自动生成测试报 告.  
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/Modules%20Frontpanel.png)  
（4）Moudule:  适用于单用例多场景连跑/单用例单场景手动测试.  
单用例多场景连跑:  点击RunModule顺序(从上到下)运行选择单条用例下所有勾选的测试场景subVi,并自动生成测试报告.   
单用例单场景手动测试:  点击RunSigleTest弹出用户选择的测试用例下的某条测试场景subVi,点击subVi前面板中RUN即开始执行测试,测试完成后,如需要保存测试报告,点击SaveResult(该测试模式测试完成后默认不保存报告),测试完成后点击Exit退出.  
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/Module%20Frontpanel.png)
* 测试界面介绍
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/Testcase%20Frontpanel.png)
* 测试报告保存
![](https://github.com/JackyCheng-ui/Labview-Automation/blob/master/img-storage/TestReport.png)
## 5.附录
*
备注：本工具为1.0版本,用户使用过程中有什么问题或者改进建议请联系Jacky Cheng修改,欢迎交流~  
THANKS ALL
