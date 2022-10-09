| 職位 | 學號 | 姓名 | 任務 |
| :---: | :---: | :---: | :---: |
| **組長** | C109118119 | [王明宇](https://github.com/yu9131) | - |
| 組員 | C109118113 | [張立揚](https://github.com/st306012) | - |
| 組員 | C109118124 | [陳柏彰](https://github.com/MoRedChen) | - |
| 組員 | C109118152 | [邱宗翰](https://github.com/muzui1115) | - |
| 組員 | C109118155 | [謝竣昊](https://github.com/HaoHsieh) | - |

```mermaid
gantt
    title 甘特圖(測試)

    section 王明宇
    專案發想 :a1, 2022-08-15, 30d
    任務分配:2022-9-15,3d
    購置硬體:a3, 2022-9-22  , 10d
    研究硬體:after a3,10d
    系統測試:a8,after a7,10d
    使用者測試:a9,after a8,5d
    
    section 張立揚
    專案發想 :a1,2022-08-15  , 30d
    任務分配:2022-9-15,3d
    購置硬體:a3, 2022-9-22  , 10d
    研究硬體:a4,after a3,10d
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
