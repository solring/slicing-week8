
# Web Slicing Practice Week 8


## 3-party library
- Swiper js: for picture/card swiper.
- Lightpicker: for customized date range picker.
- Jquery UI: for slider with 2 values.

## CSS framework
Bootstrap 4

## NOTE

### Search result頁面中的filter responsive 作法
因為假設一般user不會大幅度改動視窗大小(也就是說一打開網頁就會是phone or tablet layout)，因此這邊在phone layout的折疊式filter獨立使用了另一個form。
兩個form內input欄位的name是一樣的，因此傳回後端的key/value pair都相同，但兩個form的UI無法同步。

### 內嵌Scripts寫法
因為在排版時有將元件和頁面拆開用ejs組合，因此有些元件javascript initialization的部分是用script標籤安插在每個ejs元件的最後。
好處是很清楚這部分js程式碼是用在哪個元件上，但這樣會有很多script標h散落在最後產生的html檔案中，目前我不確定這樣的做法有沒有其他問題(e.g.不好debug?)。
之後改使用framework之後應該就可以解決這問題。