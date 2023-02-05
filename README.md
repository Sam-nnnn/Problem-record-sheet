# Problem-record-sheet
紀錄所有遇到的問題

---
ㄨ1. [ㄅㄡ本地ㄇㄧㄡ沒有errorㄑㄝㄝ，ㄣpull request卻部署失敗？](## ㄡ本地ㄇㄧㄡ沒有errorㄑㄝㄝ，ㄣpull request卻部署失敗?)

---

## ㄡ本地ㄇㄧㄡ沒有errorㄑㄝㄝ，ㄣpull request卻部署失敗?

這個問題是出自於我新執行的一個公司專案ㄝ，是一個ㄉㄩㄥ使用yarn做版本控制的專案ㄝㄋㄝ，因為ㄐㄨㄟ把檔案pull下來之後，我只有把環境run起來，並沒有執行過build,在遇到這個問題之前我都還沒有手動build過，也沒有仔細研究其部屬的過程，所以就遇到了這個問題，我本地運行的腳本都是我即時更新ㄉㄧㄜ的內容，然而ㄖㄧ部署上github的過程並未兼容我本地環境不被發現的錯誤，導致我在ㄐㄇㄩㄟcommand line or browser developer tools都沒有正確的error messageㄉㄠ，導致我一直把build失敗這件事認為是型別的erroㄐr

但是在今天也讓我發現了很多型別ㄉㄧㄜ的定義要特別注意的小眉角

```
let  = error["test"] 
ㄔㄠlet error. __test__ ㄧ
```
