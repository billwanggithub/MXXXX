# M8322 Note

## Changes
<details>
<summary>M8322BA</summary>

- [x] RPM setting is only enabled on "OOO"
- [x] disable XP1 = 0 @Shudowm mode
- [x] disable RP1 < 7 selections
- [x] 進PGM, online mode bit 不設定		
- [x] 進PGM, 0x00[7]要設為1
- [x] 0X0F[7:5]的ItemList顯示要X8
- [x] Leading angle 位置0X0F[6] -> 0x0F[4]
- [x] Alignment加圈數選項

</details>

## Notes

- Bank status(0x8E[5:4])只有在進PGM時才是正確的. 改過Bank Selection(0x8E[1:0])後的狀態是不對的
- 進PGM, online mode bit(0x86[0]) 要設定, BA版不設定
- 進PGM, auto reload off bit(0x8A[0]) 要設定. 出PGM,
    工程模式下問是否清除.非工程模式一律不清除.
    auto reload off =1, 進出PGM不會從efuse reload到register
- 0x89[6]是判斷是否close loop. 要根據這個Bit來設定FG Ratio是要填入close/open loop的設定
- 燒錄完會自動 reload efuse data, 此時TX/RX設定可會和寫入不同,需重新進PGM
- [ ] 0x8E[7:0] == 0x00才給燒錄

