# content-farm-list / 內容農場列表
主要針對香港散播假新聞那些已知的內容農場。
Mainly focused on those known content farm spreading fake news in HK.

參考報導：
* (2019-10-26) [不同網址的內容農場，背後疑由同一集團操作 - The News Lens 關鍵評論網](https://www.thenewslens.com/article/126592)

Last Update / 最後更新（2019-11-12 09xx）
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

## 注意事項
### Firefox Add-ons 權限問題
有眼利的網友指出上述 add-ons 要求頗多的權限：
* Access you data for all websites
* Access browsing history
* Access browser tabs
* Store unlimited amount of client-side data

有此擔心是絕對正常的，畢竟以上權限代表此 add-on 可以讀取你瀏覽的所有網站內容。但考慮到 add-on 功能所需，似乎不是不合理：
* 首3個權限應該是讓 add-on 可以讀取正在開啟的頁面，在正式載入內容之前檢查一下網址。而此 add-on 要有能力檢查所有網站，所以 scope 要設定為 all websites
* 第4個權限大概容許 add-on 將 blacklist/whitelist 存放在本機之內，避免因查詢而將每次瀏覽的詳請洩漏到其他伺服器，加強保障私隱亦同時增加查詢速度。

但本人未能抽空逐一檢查 source code，各位有興趣的話可以幫忙看一下。

針對這個潛在風險，可以採取以下措施：
1. 將 Firefox 設定為預設瀏覽器，瀏覽一般網站、看新聞時可以用此 add-on 檢查是否內容農場。而當有需要瀏覽重要網站時，可以轉用其他瀏覽器。此舉在手機/平板上尤其有效，在 Android 上更可不設定預設瀏覽器，每次依用途決定用哪個瀏覽器。

2. 此 add-on 是 open source，大家有懷疑可以自行檢查。當然未必可以完全防止

3. 當然如果能夠不靠這些工具自行分辨出內容農場就更好了。要分辨其實不難，通常內容農場都有以下特徵：
   * URL 看上去和其他正式網站，如新聞網站、知名論壇等有關係。也經常在域名中加入字眼暗示自己的功能，如 press 之類。
   * 標題及附圖通常很震撼，如果是為了帶風向的話，更會圍繞最熱門的話題，將內容東併西湊，然後加入一些虛假的資料。
   * 網站內通常附有大量廣告等等，文章也可能沒有出處或引用錯誤的出處
   
   
