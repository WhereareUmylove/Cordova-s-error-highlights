# Cordova-s-error-highlights
cordova的一系列莫名其妙的问题

<p><strong>1：</strong>明明配置好了android SDK, cordova run android的时候提示Cordova: Android SDK not found. Make sure that it is installed. If it is not at the default location, set the ANDROID_HOME environment variable ???这不是逗你玩吗??</p>
<ul>解决办法
<li>1:仔细检查自己的环境配置以及是否下载SDK,我的路径是C:\Users\Youngonest\AppData\Local\Android\Sdk</li>
  <li>2:当初开发corodva的一些人已经不在了，这个项目感觉几十年没人用了，BUG也没人管</li>
  <li>3:<strong>重点来了</strong>打开C:\Users\Youngonest\AppData\Local\Android\Sdk\tools这个路径下的android.bat文件，修改类容,将大概是20行和37行的target改为targets!（carodva的语法错误!!）</li>
  <li>4:我也没法子了</li>
</ul>
<p><strong>2：</strong>无法新建项目cordova create MyApp,提示啥commond faild命令行错误,<img src="./QQ图片20200113164524.png">把cordova的版本改为6.0.0就行了，cnpm i -g cordova@6.0.0,原因同样是1.2</p>
<p><strong>3：还有cordova-plugin-crosswalk-webview，我玩意我真的整吐了，我反正是不敢用了，C++和CSS的区别可能就是因为是否安装了cordova-plugin-crosswalk-webview</strong><p><b>问题</b>Failed to install 'cordova-plugin-crosswalk-webview': Error: Unhandled "error" event. </p><b>解决办法:cordova版本降到7.0.0,</b>原因同1.2</p>
<p><strong>4：</strong>Current working directory is not a Cordova-based project.这个鬼问题有很多种鬼情况，我自己都不知道自己是怎么解决的，百度一下自己查吧，当然删除项目重新创建可以解决90%的问题。至于原因我就不多少了！</p>


