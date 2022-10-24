## 組長與組員之姓名及任務
| 職位 | 學號 | 姓名 | 任務 |
| :---: | :---: | :---: | :---: |
| **組長** | C109118119 | [王明宇](https://github.com/yu9131) | - |
| 組員 | C109118113 | [張立揚](https://github.com/st306012) | - |
| 組員 | C109118124 | [陳柏彰](https://github.com/MoRedChen) | - |
| 組員 | C109118152 | [邱宗翰](https://github.com/muzui1115) | - |
| 組員 | C109118155 | [謝竣昊](https://github.com/HaoHsieh) | - |

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
任務分配 --|> 購置硬體
任務分配 --> 系統規劃
購置硬體 --|> 研究硬體
系統規劃 --> 環境建置
研究硬體 --|> 軟硬結合
軟硬結合 --|> 系統測試
系統測試 --|> 使用者測試
環境建置 --> 程式開發
程式開發 --> 網域申請
網域申請 --> 程式測試
程式測試 --> 使用者測試

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

## 功能性需求與非功能性需求(至少各三項)
功能性需求：
1. note 1
2. note 2
3. note 3

非功能性需求：
1. note 1
2. note 2
3. note 3

<br>

## 功能分解圖(functional decomposition diagram, FDD)
![功能分解圖](功能分解圖.png "功能分解圖")

<br>

## 需求分析的文字描述


<br>

## 使用案例圖
忘記密碼：
![忘記密碼](忘記密碼.png "忘記密碼")

<br>

## 使用案例說明(三個以上)
| 使用案例名稱 | 忘記密碼 |
| :-- | :-- |
| 行動者 | 使用者 |
| 說明 | 描述重設密碼之過程 |
| 完成動作 | 1. 點擊忘記密碼<br>2. 輸入信箱<br>3. 系統寄送驗證信<br>4. 點擊連結進行密碼重設 |
| 替代方法 | 1. 點擊忘記密碼<br>2. 輸入信箱<br>3. 系統判定信箱尚未註冊 |
| 先決條件 | 已經註冊過 |
| 後置條件 | 認證完畢，可以重設密碼 |
| 假設 | 無 |

| 使用案例名稱 | 案例2 |
| :-- | :-- |
| 行動者 | null |
| 說明 | null |
| 完成動作 | null |
| 替代方法 | null |
| 先決條件 | null |
| 後置條件 | null |
| 假設 | 無 |

| 使用案例名稱 | 案例3 |
| :-- | :-- |
| 行動者 | null |
| 說明 | null |
| 完成動作 | null |
| 替代方法 | null |
| 先決條件 | null |
| 後置條件 | null |
| 假設 | 無 |

<br>

## Figma使用案例動態模擬畫面
[Figma預覽連結](https://www.figma.com/proto/zs1PjkdDDMe9ZzYtN2oMWd/Untitled?node-id=3%3A2&scaling=scale-down&page-id=0%3A1&starting-point-node-id=3%3A2)

