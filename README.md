# GmtTestTool

## APP功能描述

### 第一次启动程序会要求选择芯片

![Select_Chip](assets/SelectChip.png)

### Pragramming Mode(PGM)

![Enter PGM Mode](assets/Enter_PGM.png)

<mark>PGM Mode下,若Load File時改變了TX/RX反相相關設定時會離開PGM Mode</mark>

- 進入PGM後會問你要不要做eFuse燒錄與否的檢測?
  `Yes` => 下載eFuse到register

![Confirm_CheckeFuse](assets/Confirm_CheckeFuse.png)

- 若檢測到eFuse未燒錄過會問你是否要寫入Default值
 `YES` => 寫入Default值到Register

![Confirm_SetDefaultValues](assets/Confirm_SetDefaultValues.png)

- 若測到eFuse燒錄過會問你是否要讀出Register值

![Confirm_ReadReloadRegister](assets/Confirm_ReadReloadRegister.png)

### 燒錄功能

![Burn_Pag](assets/Burn_Page.png)

- `One`烧录一个Byte : 燒錄指定的Register.
- `All`烧录全部16個Register.
- `验证`验证刻录的值是否符合GUI值.
- `Set Zero`将全部缓存器设为0.
- `Set Default`将全部缓存器设为默认值.
- `Reload`載入eFuse值到Register.不會自動讀出Register到GUI.

#### 一键刻录

<mark>需先設定RXTX極姓</mark>

```mermaid
graph LR
    A[進入PGM] --> B["設定燒錄檔的PWM(TX)/SO(TX)極性"]
    B --> C["手動改變燒錄板的TX/RX極性"]
    C --> D[執行燒錄]
    D --> E{燒錄是否成功}
```

- **CMD/SO反相**

![UART INV](assets/UART_INV.png)

- **CMD/SO无反相**

![UART_NORMAL](assets/UART_NORMAL.png)

## APP 更新下载

### 下载

**點擊[Gitee](https://gitee.com/billwang168/gmt-test-tool)頁面右側[發行版](https://gitee.com/billwang168/gmt-test-tool/releases)下載更新**

![APP_DOWNLOAD](assets/APP_DOWNLOAD.png)

### 检查/下載更新

![Check_App_Update](assets/Check_App_Update.png)

## 韧体手动更新

![Firmware_Update](assets/Firmware_Update.png)
