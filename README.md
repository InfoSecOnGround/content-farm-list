# content-farm-list / 內容農場列表
主要針對香港散播假新聞那些已知的內容農場。
Mainly focused on those known content farm spreading fake news in HK.

參考報導：
* (2019-10-26) [不同網址的內容農場，背後疑由同一集團操作 - The News Lens 關鍵評論網](https://www.thenewslens.com/article/126592)

Last Update / 最後更新（2019-11-12 08xx）
**歡迎幫忙更新**


## 所需工具
### 支援 Add-ons 的瀏覽器
#### 手機 / 平板
因為 Android 內置的 Chrome 支援 add-ons，而 iOS 的 Safari 雖支援但不清楚那個好用，大家可以考慮使用 Firefox for Mobile：
* Android: https://play.google.com/store/apps/details?id=org.mozilla.firefox
* ~~iOS: https://apps.apple.com/us/app/firefox-private-safe-browser/id989804926~~
更正：Firefox 的 iOS 版本也[不支援 Add-ons](https://support.mozilla.org/en-US/kb/add-ons-firefox-ios)，多謝網友提醒。看來只能用 Safari 的 extension，有人知道那款較好嗎？

#### 電腦
電腦的話用 Chrome / Firefox 其本上也可以可以。

Mac 的 Safari 也支援 extensions，但不知道那個比較好用。（[RoadBlock](https://apps.apple.com/us/app/roadblock-content-blocker/id1051436753) 好像不錯）

### Add-on
老實說這個部分我不在行，簡單找到這個好像不錯。

#### 終結內容農場 (Content Farm Terminator)
* GitHub: https://github.com/danny0838/content-farm-terminator
* Firefox add-on: https://addons.mozilla.org/en-US/firefox/addon/content-farm-terminator/
* Chrome Extension: https://chrome.google.com/webstore/detail/content-farm-terminator/lcghoajegeldpfkfaejegfobkapnemjl

安裝方法：
1. 使用相應的瀏覽器開啟 add-on / extensions 的連結
2. 按「安裝」

## 步驟
用不同的 Addon 方法應該大同小異，以下用 Content Farm Terminator 作例子。

以下兩種方法只需二擇其一：
* 方法1：User Blacklist
* 方法2：Web Blacklists

（無論用哪一方法，都可以自行在 User Blacklist 中額外外加上其他自訂的目標。）

### 方法1：User Blacklist
1. 瀏覽到內容農場列表：
* https://raw.githubusercontent.com/InfoSecOnGround/content-farm-list/master/hk-fake-news.txt

2. 直接將內容 copy & paste 到 User Blacklist 內就好（每行一個網域）

### 方法2：Web Blacklists
1. 先檢查一下是良好習慣：
* https://raw.githubusercontent.com/InfoSecOnGround/content-farm-list/master/hk-fake-news.txt

2. 然後 Copy & paste URL 放到 Web Blacklists：
```
https://raw.githubusercontent.com/InfoSecOnGround/content-farm-list/master/hk-fake-news.txt
```

