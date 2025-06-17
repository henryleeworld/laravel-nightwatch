# Laravel 12 守夜者

守夜者是一個託管應用程式監控平台，它為您的應用程式效能提供了無與倫比的洞察力，只有針對 Laravel 進行精心優化的系統才能提供這種智慧。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移。
```sh
$ php artisan migrate
```
- 執行 __Artisan__ 指令的 __nightwatch:agent__ 來執行守夜者代理程式。
```sh
$ php artisan nightwatch:agent
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/` 來瀏覽歡迎頁面。

----

## 畫面截圖
![](https://i.imgur.com/qeZxkF4.png)
> 快速發現應用程式的問題元件，以解決問題並最大限度減少停機時間
