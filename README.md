# Cordova-s-error-highlights
cordova的一系列莫名其妙的问题

<p><strong>1：</strong>明明配置好了android SDK, cordova run android的时候提示Cordova: Android SDK not found. Make sure that it is installed. If it is not at the default location, set the ANDROID_HOME environment variable ???这不是逗你玩吗??</p>
<ul>解决办法
<li>1:仔细检查自己的环境配置以及是否下载SDK,我的路径是C:\Users\Youngonest\AppData\Local\Android\Sdk</li>
  <li>2:当初开发corodva的一些人已经不在了，这个项目感觉几十年没人用了，BUG也没人管</li>
  <li>3:<strong>重点来了</strong>打开C:\Users\Youngonest\AppData\Local\Android\Sdk\tools这个路径下的android.bat文件，修改类容,将大概是20行和37行的target改为targets!（carodva的语法错误!!）</li>
  <li>4:我也没法子了</li>
</ul>
<p><strong>2：</strong>无法新建项目cordova create MyApp,提示啥commond faild命令行错误,把cordova的版本改为6.0.0就行了，cnpm i -g cordova@6.0.0,原因同样是1.2</p>
<p><strong>3：</strong></p>


