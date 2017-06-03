# puzzle_solver

程式說明：
首先將完整的拼圖圖案進行處理：
運用threshold 將毛邊去除，
使用erode將拼圖中間黑色邊框加粗，也手動在右側及下側讓邊框加粗

使用findContours找到每塊小塊拼圖的輪廓
再將輪廓一一畫出在新的圖形檔案上。

將所有的拼圖放在同一張圖檔上
將其中一塊拼圖「反白」，也就是將周圍塗黑，拼圖本身留白，並裁剪出一邊
之後便可運用matchTemplate找出對應的拼圖塊。

參考[附圖文件說明](https://github.com/jimmytecho/puzzle_solver/blob/master/puzzle%20solver%20%E7%A8%8B%E5%BC%8F%E8%AA%AA%E6%98%8E.pdf)
