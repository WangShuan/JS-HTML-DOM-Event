# JS-HTML-DOM-Event

  1. 焦點事件: onfocus/onblur
  
  2. 事件對象: IE瀏覽器與谷歌的event都是內置對象 可通過window.event訪問到，其他瀏覽器比如火狐 則為函數傳入的第一個參數為事件對象。
  
  3. 事件源: IE瀏覽器為 ev.srcElement ，其他瀏覽器為 ev.target
  
  4. 鼠標位置(x,y): ev.clientX 是相對於瀏覽器的距離，ev.offsetX 則是相對於事件源的距離。
  
  5. 鼠標位置小案例(拖曳): 藍色方塊是利用鼠標位置把元素以左上角為定點拖動，紫色方塊是完整拖曳。
  
  6. 事件冒泡: 事件會從當前元素一直往外層(父元素)傳遞 一直傳到window層為止。
  
  7. 焦點案例: 利用焦點來顯示/隱藏列表 點擊 Li 更改輸入框內容。
  
  8. 冒泡案例1: 點擊功能顯示列表 點擊其他地方隱藏列表。
  
  9. 冒泡案例2: 鼠標移入"分享到"滑出紅色區塊 移出隱藏紅色區塊。
  
  10. 事件源案例: 雙擊改變當前表格內容。
  
  11. 冒泡案例3：仿 select 效果。
  
  12. addEventListener: 事件捕獲，事件捕獲就是事件冒泡的相反 冒泡是由當前點擊一直往外層傳遞 捕獲則是由外層往裡傳。
  
  13. 鍵盤事件: onkeydown 配合事件對象 ev.keyCode 使用。
  
  14. 默認事件: 
      1. oncontextmenu(點擊右鍵的事件) 
      2. 阻止默認事件方法1: ev.preventDefault() || ev.returnValue = false
      3. 阻止默認事件方法2: return false
