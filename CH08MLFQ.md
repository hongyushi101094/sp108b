多級反饋佇列演算法：不需要事先知道各種程序所需要的執行時間，還可以較好地滿足各種型別程序的需要，是目前公認的一種較好的程序排程演算法。

1.排程機制：

（1）設定多個就緒佇列。在系統中設定多個就緒佇列，併為每個佇列賦予不同的優先順序，從第一個開始逐個降低。不同佇列程序中所賦予的執行時間也不同，優先順序越高，時間片越小。

（2）每個佇列都採用FCFS（先來先服務）演算法。輪到該程序執行時，若在該時間片內完成，便撤離作業系統，否則排程程式將其轉入第二佇列的末尾等待排程，.......。若程序最後被調到第N佇列中時，便採用RR方式執行。

（3）按佇列優先順序排程。排程按照優先順序最高佇列中諸程序執行，僅當第一佇列空閒時才排程第二佇列程序執行。若優先順序低佇列執行中有優先順序高佇列程序執行，應立刻將此程序放入佇列末尾，把處理機分配給新到高優先順序程序。

2.實時排程演算法按排程方式分為：

①非搶佔式排程演算法②搶佔式排程演算法

非搶佔式演算法：

（1）非搶佔式輪轉排程演算法。

（2）非搶佔式優先排程演算法。

搶佔式排程算：

（1）基於時鐘中斷的搶佔式優先順序排程演算法。

（2）立即搶佔的優先順序排程演算法。-------出自https://www.itread01.com/content/1545101124.html
