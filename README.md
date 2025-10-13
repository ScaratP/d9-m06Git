# 10月 AI小聚 開源
---
### 我們在幹嘛
打造一款專為國立臺東大學學生設計的 Android 應用程式，旨在整合多項校園生活與學習所需的功能。

本專案使用 Android Studio (Kotlin) 進行開發，旨在提供一個全面且便利的數位校園體驗，功能涵蓋學習管理、校園資訊獲取，乃至於日常生活輔助。

### 核心功能
本應用程式包含了以下六大模組：

1. 🎓 課表管理
    
    - 資料獲取： 利用網頁爬蟲技術，抓取使用者登入後學校教務系統/選課系統的課表資訊。
      
2. ⏰上課通知提醒

    - 貼心提醒： 透過 Android Notification 服務，提供上課前自動提醒功能。

3. ✅ 出缺勤紀錄

    - 資料同步： 利用網頁爬蟲技術，抓取並顯示使用者在請假系統中的出缺勤紀錄。

4. 🗺️ 智慧校園定位導航

    - 室外定位導航： 整合 Google Maps API，提供校園周邊及室外區域的定位與導航服務。
    
    - 室內定位： 透過掃描當前wifi資訊並訓練模型，提升在室內環境下的定位準確率。
    
    - 室內最短路徑導航： 採用圖片辨識技術，識別走廊、牆壁、教室等元素，並計算出最短的室內移動路徑。

5. 📝 課程筆記

    - 功能： 提供功能完整的筆記編輯器，支援富文本編輯功能，方便學生隨時紀錄課程重點。
    
    - *註：此功能是基於現有開源專案程式碼進行修改與整合。*

6. 🍔 學餐隨機選擇

    - 娛樂功能： 簡單的轉盤隨機選擇功能，幫助有「選擇困難症」的使用者快速決定午餐或晚餐地點。

### 技術實現
| 功能模組	| 開發環境/語言 | 核心技術/API | 備註 |
| -- | -- | -- | -- |
| 主程式 | Android Studio (Kotlin) | - |	- |
| 課表/出缺勤	| Kotlin/python | 網頁爬蟲技術	| 需處理登入狀態及資料解析。|
| 上課通知 |	Kotlin |	Android Notification API	| - |
| 室外定位導航 |	Kotlin | Google Maps API	| 標準地圖服務集成。|
| 室內定位 |	python |	機器學習模型 | (自訓練)	專注於高準確率的室內定位。|
| 室內導航	| Kotlin |	圖片辨識/最短路徑演算法 | 利用電腦視覺處理室內結構。|
| 課程筆記	| Kotlin |	富文本編輯器 (改寫) | - |
| 學餐隨機	| Kotlin |	轉盤/亂數生成演算法	| - |

### 成果 
|功能	|截圖|
|--|--|
|課表與通知|<img width="25%" height="25%" alt="image" src="https://github.com/user-attachments/assets/26cd0656-905c-4bbb-9202-16894da21963" />|
|請假管理|<img width="25%" height="25%" alt="image" src="https://github.com/user-attachments/assets/f160f882-2f64-4862-b262-5800031d9af9" />|
|學餐隨機|<img width="25%" height="25%" alt="image" src="https://github.com/user-attachments/assets/2a75c922-2ab4-4e67-8a08-eee0f8071031" />|

### 原始碼請求 (Request Source Code)
因應學校活動需求，本專案目前只公開功能說明與完成截圖。


### Reference
- Android Developers Documentation
- Google Maps Platform API


