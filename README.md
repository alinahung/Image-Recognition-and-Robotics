## 負責項目

1. App 影像辨識卡牌
2. 建立 micro:bit 的藍芽連線並傳送指令。

## 軟體

1. MIT App Inventor（開發手機 APP）
2. Personal Image Classifier (PIC) Tools（影像辨識訓練）
3. MakeCode（編寫micro:bit小車的程式）
4. Python（Linebot 聊天機器人建立）

## 硬體

- Android 手機 * 1
- 麥坤小車
- 地圖
- 桌遊卡牌
- 辨識區

### 功能

1. **影像辨識卡牌**：對卡牌進行影像辨識，判斷其前、後、左、右方向。
2. **結果傳輸**：將辨識到的卡牌結果（前、後、左、右）傳送給 micro:bit 小車。
3. **小車控制**：micro:bit 控制小車穩定地前進，根據指令精確移動。
4. **移動判定**：在線上地圖中進行移動判定，判斷前方是否有障礙物或資源。
5. **任務卡與資源記錄**：使用 Linebot 建立任務卡，並記錄比賽過程中獲取的資源。

## 執行流程

1. **Linebot 任務卡**：Linebot 隨機抽取任務卡。
2. **影像辨識**：透過手機 APP 進行影像辨識，判斷卡牌方向（前、後、左、右）。
3. **小車移動**：麥坤小車根據指令進行移動，遇到障礙物則停止。
4. **資源顯示**：Linebot 顯示玩家收集到的資源。

## 遇到的問題與解決方式

- **問題**：micro:bit 的藍芽連線不穩定，將值一次性傳給 micro:bit，使用者操作錯誤導致接收指令有誤。
- **解決方式**：
  1. 更新藍牙版本套件以提升穩定性。
  2. 以陣列形式傳送方向指令，增強傳輸可靠性。
  3. 使用 `if_else` 函式處理使用者操作按鈕的介面設計，減少操作錯誤。

## 實作影片
https://github.com/user-attachments/assets/1bc258c3-9a86-483c-b101-c1ce7b18ddc1

