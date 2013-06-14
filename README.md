#StrokesPlus 说明文档
这里是一些自用的 [StrokesPlus](http://www.strokesplus.com/forum/6/downloads/) 手势代码,包括简单的直接模拟快捷键以及一些自写**特殊功能**

###我的配置文件
+ [StrokesPlus.lua](https://github.com/defpt/StrokesPlus/blob/master/StrokesPlus.lua) 是全局执行的脚本文件
+ [StrokesPlus.xml](https://github.com/defpt/StrokesPlus/blob/master/StrokesPlus.xml) 是所有自定义手势设置
+ [RenameBackup.bat](https://github.com/defpt/StrokesPlus/blob/master/RenameBackup.bat) 是备份文件重命名为原文件的批处理

###主要有如下几个：

+ [AutoScroll](https://github.com/defpt/StrokesPlus/blob/master/AutoScroll.lua) 自动滚屏，每次滚动一个屏幕。**要手势激活**，默认鼠标移动到桌面左侧(大概一个Win8任务栏宽度)可退出激活状态，可自己按需修改
+ [Clip2OneNote](https://github.com/defpt/StrokesPlus/blob/master/Clip2OneNote) 发送到 OneNote 包括两个版本，一个要设置路径，一个不需设置路径
+ [OpenLinkorNewTab](https://github.com/defpt/StrokesPlus/blob/master/OpenLinkorNewTab.lua) 新建标签或者新标签后台打开链接
+ [OpenLinkorSearchText](https://github.com/defpt/StrokesPlus/blob/master/OpenLinkorSearchText.lua) 搜索选中内容或者新标签前台打开链接
+ [OpeninGoogleWebeCache](https://github.com/defpt/StrokesPlus/blob/master/OpeninGoogleWebeCache.lua) 用谷歌快照功能打开网页
+ [ScrollWithMouse](https://github.com/defpt/StrokesPlus/blob/master/ScrollwithMouse.lua) 划手势激活，光标移到滚动条滑块即可拖动鼠标进行自由滚动，鼠标移到桌面底部退出激活状态，可自己按需修改。**特别注意由于采用了滚动块颜色判定，***所以如过使用自定义滚动条要自己修改颜色代码*
+ [SearchInWebsite](https://github.com/defpt/StrokesPlus/blob/master/Searchinwebsite.lua) 站内搜索，默认用的是谷歌引擎
+ [SearchThisWithGoogle](https://github.com/defpt/StrokesPlus/blob/master/Searchthiswithgoogle.lua) 谷歌搜索，**全局搜索利器**，在记事本、word等文本编辑器也可使用
+ [Shutdown](https://github.com/defpt/StrokesPlus/blob/master/Shutdown.lua) 关机
+ [SupperForward](https://github.com/defpt/StrokesPlus/blob/master/SupperForward.lua)、[SupperBack](https://github.com/defpt/StrokesPlus/blob/master/SupperBack.lua) 前进、后退，外加了模拟键盘左右方向键
+ [TranslateThisWithGoogle](https://github.com/defpt/StrokesPlus/blob/master/Translatethiswithgoogle.lua) 谷歌翻译，**全局利器**，默认自动识别翻译为中文，可自己设置默认翻译语言
+ [ViewWithIE](https://github.com/defpt/StrokesPlus/blob/master/ViewwithIE.lua)、[ViewWithFirefox](https://github.com/defpt/StrokesPlus/blob/master/ViewwithFirefox.lua)、[ViewWithChrome](https://github.com/defpt/StrokesPlus/blob/master/Viewwithchrome.lua) 使用别的浏览器打开当前网页
+ [JSTools](https://github.com/defpt/StrokesPlus/blob/master/JSTools.lua)  Firefox上调用小书签代码的模板,不过要配合启用地址栏可运行代码才行，可通过扩展（比如tab_utilities） 或脚本（uc脚本）总在当前标签页打开Bookmarklet，代码为：

          eval("openLinkIn = " + openLinkIn.toString().replace(/(?=if \(where == "save"\))/, 'if (url.substr(0, 11) == "javascript:") where = "current";').replace(/(?=var loadInBackground)/, 'if (w.gBrowser.currentURI.spec == "about:blank" && !w.gBrowser.mCurrentTab.hasAttribute("busy")) where = "current";'));
      
###所有功能效果图
![](https://github.com/defpt/StrokesPlus/blob/master/StrokesPlus.png?raw=true)