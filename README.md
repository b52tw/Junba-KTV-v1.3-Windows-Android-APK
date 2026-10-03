# 峻爸 KTV 多文字軌核對器 v1.3｜純離線穩定版

這是一支獨立的錄音＋逐字稿核對播放器，不負責重新做語音辨識，也不會把錄音或文字上傳雲端。

## 主要功能
- Windows 10/11 Single EXE
- Android APK
- 載入 M4A/MP3/WAV 等錄音
- 載入 DOCX/SRT/VTT/TXT/JSON/CSV/HTML 文字軌
- 上方完整全文 KTV 反白
- 下方時間軸同步定位
- 上方 KTV 與下方時間軸可獨立停止／恢復跟隨
- 多文字軌比對；核對顏色只顯示在結果欄，不遮字幕
- 時間重疊合併比對，降低因不同斷句造成的假性「漏字」
- 離線 HTML KTV 網頁包、SRT/VTT 匯出、專案儲存

## 關於「漏字」
本程式只核對既有文字，不重新聽音訊辨識。紅色表示兩個文字軌在同一時間窗的差異較大，不代表一定真的漏字。v1.3 已把原本「只找一個中點段落」改成「合併所有時間重疊段落」，可明顯降低因兩份字幕斷句方式不同造成的誤判。真正有沒有漏字，仍以播放錄音人工確認為準。

## GitHub Actions
使用 `.github/workflows/build-windows-android-v1.3.yml`。成功後產生：
- `Junba-KTV-MultiTrack-v1.3-Single-EXE-Windows-x64`
- `Junba-KTV-MultiTrack-v1.3-Android-APK`
