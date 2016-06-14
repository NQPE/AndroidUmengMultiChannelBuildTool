# AndroidUmengMultiChannelBuildTool
基于美团Android自动化之旅—生成渠道包之java版打包工具</br>

如果各位还在为打umeng的各种渠道包烦恼，那么这里推荐大家参考一下
<a target="_blank" href="http://tech.meituan.com/mt-apk-packaging.html">美团渠道打包方案</a> 

本文是根据这个方案写的一个打包工具 因为在原文中美团给出的是用python来写打包工具 需要大家安装python环境

个人觉得比较麻烦，所以就自己写了一个基于java的GUI打包工具，使用也是相当简单

1.AndroidManifest.xml中设置umeng渠道的那个注释掉</br>
<img src="https://github.com/NQPE/AndroidUmengMultiChannelBuildTool/blob/master/Pics/1.png?raw=true"/></br>
2.在你的自定义的application中用java代码设置umeng渠道号</br>
<a target="_blank" href="http://tech.meituan.com/mt-apk-packaging.html">具体java代码在utils里</a> 
<img src="https://github.com/NQPE/AndroidUmengMultiChannelBuildTool/blob/master/Pics/2.png?raw=true"/></br>
3.编译你的项目为APK  然后使用所给的工具包 选择你的APK路径</br>
（注意这里的工具为jar文件 如果下载后双击不出现GUI界面 请单击选择打开方式 然后选择打开jar包的打开方式）</br>
其中里面的渠道号可以打包多个 比如可以输入  360;wandoujia;baidu  (以分号隔离)

打好的包就是在你的APK同路径下
<img src="https://github.com/NQPE/AndroidUmengMultiChannelBuildTool/blob/master/Pics/4.png?raw=true"/></br>

*如果需要python工具的可参考这篇文章</br>
<a target="_blank" href="https://github.com/GavinCT/AndroidMultiChannelBuildTool">安卓多渠道打包工具。</a> 
