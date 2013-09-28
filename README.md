# Addons for Statamic

集中將會使用到的 Statamic Addons 集中存放，以 Git Submodule 方式維護。

由於 Addons 的安裝並不是單一目錄模式，部分外掛除了擺進根目錄下的 `_Add-ons` 之外，還有可能需要同時在 `_config` 目錄下的 `add-ons` 添加檔案，或是額外建立單獨的目錄（例如 Raven 就需要新建 `_config/formsets` 目錄），因此無法將外掛均以 Git Submodule 形式掛進專案。

當 Statamic 更成熟之後，理應設計出更方便的外掛安裝架構（類似 Wordpress 的「在程式內安裝、升級」，或是乾脆如 Symphony CMS 般通通使用 Git Submodules）。

## Statamic Version

目前為 1.6.4。

預計 1.7 將會加入前端會員登入與管理功能。

## 外掛列表

1. [Raven](http://www.statamic.com/add-ons/raven)：官方付費外掛（每站 $49），與 Symphony CMS 的 Events 相近，以 HTML Forms 處理要送進網站的各項處理。（不在此倉儲中管理）
2. [Bison](http://builtwithbison.com)：尚未正式釋出的電子商務外掛，應該會是付費使用。
3. [Mobile Detect](https://github.com/sergeifilippov/statamic-mobile-detect)：整合 [Mobile Detect](https://github.com/serbanghita/Mobile-Detect) 功能，使用核心標籤 `{{ mobile_detect }}` 在模板中判斷 computer、tablet 與 phone 三種使用者代理，進而讓伺服器吐出對應的內容。（目錄下有使用 Mobile Detect 倉儲作為 submodule，但遞歸更新總是失敗，要記得進入確實拉回該目錄下的資料。）