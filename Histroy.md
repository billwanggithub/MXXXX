# Histroy

- V1.0.9152.13527`250121`
`FW:24121900`
  - 優化Registes操作
  - 優化APP更新機制
  - 優化USB R/W Handling
  - 加入CRC-16檢查
  - 優化一鍵燒錄
  - clamp start/stop/Close2Open/Open2Closep Points to 100%

- V1.0.9138.12570 `250107`
`FW:24121900`
  - Confirm check eFuse/set default when entering PGM Mode
  
- V1.0.9137.12539 `250106`
`FW:24121900`
  - Check if Lost connection on PGM Mode
  - Fix PGM => POWER OFF => NONE => POWER ON => PGM 當機問題
  - Fix PGM => POWER OFF => POWER ON => Online Test 無反應
  - [M8421]Fix soft switch GUI

- V1.0.9137.12462  `250106`
`FW:24121900`
  - 檢查無燒錄時填入default Values
  - Change checksum to CRC16
  - 自動檢查APP/Firmware更新
  - 存檔加入CRC,時間至檔名
  - Add Tx/Rx inverted options to AutoBurn
  - Disable all function when Load Csv file
  - Add Align Output Duty change time to others GUI
  - Hide Auto Reload Bit
  - set Auto Reload Bit when entering PGM mode
  - Improve None ⇔ Online Mode Stability
  - Fix Bug: PWM is high after PGM/Online Mode fail
  - Add Load/Save Button on toolbar
  - 跳到8322在跳回8421會當掉 =>Done
  - [M8322]
    - 轉速曲線下新增的點數標示示意圖
    - 進 online test  時，default 值寫入 Register
    - Update  M8322AB registers
    - Add Leading Angle to Output Driving Setting GUI
    - Add AutoBurn
    - Add Burn Repeat command
  - [M8421]
    - Check Min > max PRM
    - ocp_offset 為high，等改版後再預設為0
  