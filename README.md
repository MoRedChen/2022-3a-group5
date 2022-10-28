## 組長與組員之姓名及任務
| 職位 | 學號 | 姓名 | 任務 |
| :---: | :---: | :---: | :---: |
| **組長** | C109118119 | [王明宇](https://github.com/yu9131) | 管理專案進度 |
| 組員 | C109118113 | [張立揚](https://github.com/st306012) | 硬體功能開發 |
| 組員 | C109118124 | [陳柏彰](https://github.com/MoRedChen) | 程式編寫 |
| 組員 | C109118152 | [邱宗翰](https://github.com/muzui1115) | 軟硬體結合 |
| 組員 | C109118155 | [謝竣昊](https://github.com/HaoHsieh) | 軟硬體結合 |

<br>

## 甘特圖
```mermaid
gantt
    title 甘特圖(測試)
    section 王明宇
    專案發想 :a1, 2022-08-15, 30d
    任務分配:2022-9-15,3d
    購置硬體:a3, 2022-9-22  , 10d
    研究硬體:after a3,10d
    軟硬結合: 2022-11-06 ,20d
    系統測試:a8,after a7,10d
    使用者測試:a9,after a8,5d
    
    section 張立揚
    專案發想 :a1,2022-08-15  , 30d
    任務分配:2022-9-15,3d
    購置硬體:a3, 2022-9-22  , 10d
    研究硬體:a4,after a3,10d
    軟硬結合: 2022-11-06 ,20d
    系統測試:after a7,10d
    使用者測試:a9,after a8,5d
    
    section 陳柏彰
    專案發想 :a1,2022-08-15, 30d
    任務分配:2022-9-15,3d
    系統規劃: a3,2022-9-20,15d
    環境建置:a4,after a3,5d
    程式開發:a5,after a4,50d
    網域申請:a6,after a5,5d
    程式測試:a7,after a6,10d
    使用者測試:a9,after a8,5d
      
    section 邱宗翰
    任務分配:2022-9-15,3d
    系統規劃: a2,2022-9-20,15d
    環境建置:after a3,5d
    程式開發:a5,after a4,50d
    程式測試:a7,after a6,10d
    使用者測試:a9,after a8,5d
    
    section 謝竣昊
    任務分配:2022-9-15,3d
    系統規劃: a2,2022-9-20,15d
    環境建置:after a2,5d
    程式開發:a5,after a4,50d
    程式測試:a7,after a6,10d
    使用者測試:a9,after a8,5d
```

<br>

## PERT/CPM圖
```mermaid
classDiagram

專案發想 --|> 任務分配
任務分配 --> 購置硬體
任務分配 --|> 系統規劃
購置硬體 --> 研究硬體
系統規劃 --|> 環境建置
研究硬體 --> 軟硬結合
軟硬結合 --> 系統測試
系統測試 --> 使用者測試
環境建置 --|> 程式開發
程式開發 --|> 網域申請
網域申請 --|> 程式測試
程式測試 --|> 使用者測試

專案發想:開始：2022-08-15
專案發想:結束：2022-09-14
專案發想:需時：30d

任務分配:開始：2022-09-15
任務分配:結束：2022-09-17
任務分配:需時：3d

購置硬體:開始：2022-09-22
購置硬體:結束：2022-10-01
購置硬體:需時：10d

研究硬體:開始：2022-10-03
研究硬體:結束：2022-10-12
研究硬體:需時：10d

軟硬結合:開始：2022-11-06
軟硬結合:結束：2022-11-25
軟硬結合:需時：20d

系統規劃:開始：2022-09-20
系統規劃:結束：2022-10-04
系統規劃:需時：15d

環境建置:開始：2022-10-05
環境建置:結束：2022-10-09
環境建置:需時：5d

程式開發:開始：2022-10-10
程式開發:結束：2022-11-28
程式開發:需時：50d

網域申請:開始：2022-11-29
網域申請:結束：2022-12-03
網域申請:需時：5d

程式測試:開始：2022-12-04
程式測試:結束：2022-12-13
程式測試:需時：10d

系統測試:開始：2022-12-14
系統測試:結束：2022-12-23
系統測試:需時：10d

使用者測試:開始：2022-12-24
使用者測試:結束：2022-12-28
使用者測試:需時：5d
```

<br>

## 功能性需求與非功能性需求
功能性需求：
1. 查詢該店存貨量
2. 查詢附近存貨
3. 會員可預定商品

非功能性需求：
1. 使用性(usability)：導入Google Map，較易上手
2. 維護性(maintainability)：硬體部分占比少，較易維護
3. 可靠度(reliability)：導入Google Map，較穩定

<br>

## 功能分解圖(functional decomposition diagram, FDD)
![功能分解圖](功能分解圖.png "功能分解圖")

<br>

## 需求分析的文字描述
一個存貨查詢系統的需求分析簡述如下：
1. 使用者可以藉由載入(Load) 貨品清單(Inventory) 資料來產生報表(Inventory Reports)。
2. 使用者可以藉由載入以及儲存貨品資料。
3. 銷售人員(Sales Clerk) 紀錄現場的貨品銷售。
4. 任何銷售必須更新存貨。
5. 如果該店無存貨，將會搜尋附近有存貨之店家。

<br>

## 使用案例圖
忘記密碼：
![忘記密碼](忘記密碼.png "忘記密碼")

<br>

## 使用案例說明
| 使用案例名稱 | 忘記密碼 |
| :-- | :-- |
| 行動者 | 使用者 |
| 說明 | 描述重設密碼之過程 |
| 完成動作 | 1. 點擊忘記密碼<br>2. 輸入信箱<br>3. 系統寄送驗證信<br>4. 點擊連結進行密碼重設 |
| 替代方法 | 1. 點擊忘記密碼<br>2. 輸入信箱<br>3. 系統判定信箱尚未註冊 |
| 先決條件 | 已經註冊過 |
| 後置條件 | 認證完畢，可以重設密碼 |
| 假設 | 無 |

| 使用案例名稱 | 登入系統 |
| :-- | :-- |
| 行動者 | 使用者 |
| 說明 | 顧客輸入帳號密碼進入系統 |
| 完成動作 | 1. 點擊信箱欄輸入帳號<br>2. 點擊密碼欄輸入密碼<br>3. 點擊登入<br>4. 進入首頁 |
| 替代方法 | 1. 點擊信箱欄輸入帳號<br>2. 點擊密碼欄輸入密碼<br>3. 點擊登入<br>4. 提示帳號密碼有誤 |
| 先決條件 | 無 |
| 後置條件 | 登入系統成功進行查詢 |
| 假設 | 無 |

| 使用案例名稱 | 存貨查詢 |
| :-- | :-- |
| 行動者 | 使用者 |
| 說明 | 顧客查詢所需商品之存貨 |
| 完成動作 | 1. 點擊查詢存貨<br>2. 輸入商品名稱<br>3. 顯示該店庫存數量<br> |
| 替代方法 | 1. 點擊查詢存貨<br>2. 輸入商品名稱<br>3. 該店查無此商品<br> |
| 先決條件 | 已完成登入系統 |
| 後置條件 | 查詢附近庫存 |
| 假設 | 無 |

<br>

## Figma使用案例動態模擬畫面
[Figma預覽連結](https://www.figma.com/proto/zs1PjkdDDMe9ZzYtN2oMWd/Untitled?node-id=3%3A2&scaling=scale-down&page-id=0%3A1&starting-point-node-id=3%3A2)

