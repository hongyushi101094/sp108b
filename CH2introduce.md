CH2 introduce

作業系統是一個讓程式運行變簡單的軟件甚至能夠同時運行程序。


一個正在運行的程序會做一件非常簡單的事情：

執行指令。處理器從內存中獲取（fetch）一條指令，對其進行解碼（decode）（弄清楚這是哪條指令），然後執行（execute）它（做它應該做的事情，如兩個數相加、訪問內存、檢查條件、跳轉到函數等）。完成這條指令後，處理器繼續執行下一條指令，依此類推，直到程序最終完成①。----出至Operating Systems: Three Easy Pieces 中文版

作業系統能共享內存讓程式更加簡化，還有能夠與設備交互成運行等等。但是要做到這些作業系統需要利用一種叫做虛擬化的技術!


操作系統將物理（physical）資源（如處理器、內存或磁盤）轉換為更通用、更
強大且更易於使用的虛擬形式。因此，我們有時將操作系統稱為虛擬機（virtual machine）。----出至Operating Systems: Three Easy Pieces 中文版


作業系統的幾個主題:

1.虛擬化CPU:在一些硬件的幫助下，讓CPU看起來有很多個在處理程序，但其實只是假象，事實上還是只有一個CPU的存在，只是作業系統把CPU轉換成多個CPU的假象。

2.虛擬化內存:作業系統在原本物理內存的地址建立一個虛擬地址供程序共享，但並不是使用物理內存裡的地址，而是使用虛擬化內存裡的地址。

3.並發:在作業系統中，併發是指一個時間段中有幾個程式都處於已啟動執行到執行完畢之間，且這幾個程式都是在同一個處理機上執行，但任一個時刻點上只有一個程式在處理機上執行。
--來自https://www.itread01.com/content/1541221446.html


4.持久性:系統內存容易丟失數據，所以需要硬件加上作業系統來持久的保存數據，作業系統裡管理磁碟的軟件為文件系統，不同於虛擬化CPU 虛擬化內存文件
，文件系統不會建立虛擬磁盤，文件系統是一種儲存和組織電腦資料的方法，它使得對其存取和尋找變得容易
