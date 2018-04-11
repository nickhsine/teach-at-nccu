### 網頁、載具與影像（片）
影像（片）的品質好 -> 影像（片）的檔案大 -> 網路傳輸慢 -> 網頁 loading 久 -> 使用者不耐煩 -> 使用者不等了

影像（片）的品質差 -> 影像（片）的檔案小 -> 網路傳輸快 -> 網頁 loading 快 -> 使用者看到了 -> 但品質怎麼這麼差？

載具小 -> 需要的影像（片）小 

載具直擺 -> 不要給橫幅的照片

載具大 -> 需要給解析度高的影像（片）

載具橫擺 -> 不要給直擺的照片

要如何在影像（片）的品質與網頁的呈現取得平衡，需要雙方的協調與努力。

### 呈現
#### Responsive image （響應式圖片）
**根據載具的長寬比不同，選則不同長寬比的照片呈現。**

例子：[20年了　香港，你好嗎？](https://www.twreporter.org/topics/transfer-of-sovereignty-over-hong-kong-20years)

優點：<br/>
手機直擺 -> 給直圖。<br/>
手機橫擺 -> 給橫圖。<br/>
照片的比例隨著螢幕的比例 -> 照片不會被裁切。

#### Resolution switching
**根據載具的螢幕解析度，選擇不同大小的照片呈現。**

例子：[英國衛報](https://www.theguardian.com/international)

優點：<br/>
手機螢幕小 -> 給小圖。<br/>
手機螢幕大 -> 給大圖。<br/>
照片的畫質隨著螢幕的大小跟動 -> 省網路頻寬 -> 網頁呈現速度提升。

#### Progressive image
**先讓使用者看小圖，再漸變成解析度高的大圖**
例子：[medium](https://medium.com/)

優點：<br/>
小圖 -> 速度快 -> 使用者先看到 -> 瀏覽器再慢慢載入大圖<br/>
提升使用者經驗。

### 裁切與壓縮
**基本四種裁切(根據網站設計，長寬也會有所不同)**<br/>
1. tiny (w: 150px)
2. mobile (w: 800px)
3. tablet (w: 1200px)
4. desktop (w: 1800px)

由於網頁特性，影像上儘量給橫圖。

裁切、壓縮影像的好工具：
[imagemagick](http://b8807053.pixnet.net/blog/post/337965926-imagemagick)

轉檔、壓縮影片的好工具：
[ffmpeg](https://lnpcd.blogspot.tw/2012/09/ffmpeg.html)

### 技術上的限制
#### 影片
* 檔案格式<br/>
各個瀏覽器之間可支援的影片[檔案格式不同](https://www.w3schools.com/tags/tag_video.asp)。<br/>
所以影片至少要轉出 `webm` 和 `MPEG-4/H.264` 的檔案格式。

* 自動播放(autoplay)<br/>
  * iPhone, iPad 等行動載具不提供自動播放。要自動播放，可以，但要靜音。
  
* 舊的瀏覽器的枷鎖
  * 有些舊的瀏覽器像是 IE(11)，要透過程式碼去操控影片不易。
