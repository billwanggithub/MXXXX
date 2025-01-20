# GmtTestTool

## APP 更新下载

### 下载

**點擊[Gitee](https://gitee.com/billwang168/gmt-test-tool)頁面右側[發行版](https://gitee.com/billwang168/gmt-test-tool/releases)下載更新**

![APP_DOWNLOAD](assets/APP_DOWNLOAD.png)

### 检查/下載更新

![Check_App_Update](assets/Check_App_Update.png)

## APP功能描述

### 第一次启动程序会要求选择芯片

![Select_Chip](assets/SelectChip.png)

### Pragramming Mode(PGM)

![Enter PGM Mode](assets/Enter_PGM.png)

 >Note: 若Load File時改變了TX/RX反相相關設定時會離開PGM Mode

- 進入PGM後會問你要不要做eFuse燒錄與否的檢測?
  `Yes` => 下載eFuse到register
  
![Confirm_CheckeFuse](assets/Confirm_CheckeFuse.png)

- 若檢測到eFuse未燒錄過會問你是否要寫入Default值
 `YES` => 寫入Default值到Register

![Confirm_SetDefaultValues](assets/Confirm_SetDefaultValues.png)

### 燒錄功能

![Burn_Pag](assets/Burn_Page.png)

### 一键刻录

- **CMD/SO反相**

![UART INV](assets/UART_INV.png)

- **CMD/SO无反相**

![UART NORMAL](assets/UART_NORMAL.png)

## 韧体手动更新

![Firmware_Update](assets/Firmware_Update.png)
