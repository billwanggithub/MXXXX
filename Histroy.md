# Histroy

V1.0.9217.14963`250327`
`FW:25032600`
  - Alignment加圈數選項

- V1.0.9217.14937`250327`
`FW:25032600`
- Fix 切換Programmer/Burn分頁時,Register Map不見問題
- Fix 没接调试板时演示一键烧录流程，打开 TX/RX 自动，load file，最后点击取消后，软体会宕机
- 工程模式下,離開PGM時,詢問要不要清除Auto reload bit

- V1.0.9216.14920`250326`
`FW:25032600`
  - Update M8322BA register stuff

- V1.0.9216.14908`250326`
`FW:25032600`
  - kill all process when exit APP
  - update new firmware V25032600(離線燒錄可重覆燒錄TX/RX有反相)
  - show CRC in one-click-burn

- V1.0.9214.14875`250324`
`FW:25031900`
  - M8322
    - Fix One-Click-Burning Problem when power is always ON

- V1.0.9210.14825`250320`
`FW:25031900`
  - increase online test RPM throughput
  - Fix 0x86, 0x8A PGM problem

- V1.0.9209.14820`250319`
`FW:25031900`
  - Show MessageBox to TopMost
  - Fix Read RPM Error Message after Exit Online TEst

- V1.0.9209.14811`250319`
`FW:25031900`
  - Improve R/W register stability
  - Improve read RPM speed @ online test
  - Check Programmer Mode

- V1.0.9204.14708`250314`
`FW:25031200`
  - Add Offline Burn
  - Fix One-Click Burn Bug
  - Update M8323BA watchdog stuff
  - Fix UART not work after PWM init
  - Change UART Config as Init  
  - [M8323]Add Enter PGM
  - update new FW 25031200

- V1.0.9194.14468`250304`
`FW:24121900`
  - [M8421]Add RPM difference debug

- V1.0.9188.14349`250226`
`FW:24121900`
  - Fix M8421 MinRpmSetting check range bug

- V1.0.9182.14302`250220`
`FW:24121900`
  - Add M8421 XP1/Xp2/YP1/YP2/RP1/RP2 sweep

- V1.0.9182.14288`250220`
`FW:24121900`
  - Fix empty check error if GUI autoreload bit is set before Enter PGM
  - When enter PGM, UART polarity check begin from GUI TX/RX inv setting
  - Fix Online test jump to PGM, no reset WDT command

- V1.0.9182.14280`250220`
`FW:24121900`
  - don't update GUI when checking efuse

- V1.0.9181.14278`250219`
`FW:24121900`
  - Fix Query/Wtite不同步衝突問題
  - Fix UART Test tool no display on reading  
  - 跳出PGM後,TX/RX INV切回不反向

- V1.0.9175.14227`250213`
`FW:24121900`
  - 自動切換TX/RX極性
  - TX/RX polarity auto switching when CMD/SO register changing
  - Add Read Protection
  - Fix check PGM data pattern
  - Add burned chip Read Protection 
  - Fix Rolling Test Window
  - Fix online test bit only set @first run
  - Fix WDT/Read RPM timing async to eliminate RPM glitch
  - Save Language Setting
  - Optimize Update Firmware GUI
  - Optimize the downlaod file

- V1.0.9154.13653`250123`
`FW:24121900`
  - Fix IsAutoWrite = false, Field not Updated
  - [GXXXX]Add 0xF2,0XF3

- V1.0.9154.13647`250123`
`FW:24121900`
  - Fix GUI CRC Update error
  - Fix無AutoWrite時，Reg改變, field值沒有變化
  - Fix 改變值時,重複寫Register
  - autosave i2c/uart setting @ applicationsetting.ini

- V1.0.9153.13587`250122`
`FW:24121900`
  - Add Default/Zero to Register Page
  - Speed Curve增加AutoScale按鍵

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
  