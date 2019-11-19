# Gomuku

[Demo Link](https://ponchimeow.github.io/Gomuku/)

## 概述

分為兩個 component，棋盤與棋子，畫面以`<canvas>`繪製

```
render() {
    return (
      <div className='wrapper'>
        <Board />
        <Chess />
      </div >
    );
  }
```

`<Board />`僅繪製棋盤，無其他處理

`<Canvas />`，與棋盤大小相同，設置`onClick event`監測，點擊後計算點擊位置相對應棋盤的座標

座標紀錄於`chessLogs`中以陣列儲存，`render()`時判斷獲勝者
