首先:進成為一個動態的過程，又可以說為運行中的程序
之後關於虛擬化CPU的原理為，一個時間片段執行一個進程，讓其看起來像是同時進行，文章說其為时分共
享（time sharing）CPU 技术，但是進行十分共享時會消耗性能，所以需要在十分共享跟性能中取一個中間值

1.程序轉化成進程:
![image](https://github.com/hongyushi101094/sp108b/blob/master/01.png)----來自Operating Systems: Three Easy Pieces 中文版

如圖所示首先將代碼跟靜態數據堆家載到內存中，然後加載到進程的地址空間中，之後還要分配內存從而程序才能開始。
