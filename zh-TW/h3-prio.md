# HTTP/3 優先次序 ( Prioritization )

如前所述，串流之間的優先級已從主要的 HTTP/3 規範中刪除，之後會分開處理。

這是從 HTTP/2 優先級排序模型中學到的東西，以及它在現實世界中的實現（ 或缺少 ）。

[一個比HTTP/2更簡單的優先級模型](https://tools.ietf.org/html/draft-ietf-httpbis-priority)
使用 HTTP 標頭字段和有限數量的優先級設置。這是對 HTTP/2 標頭 frame 中的 "相依關係"和"權重"標誌的關鍵更改，並使其在應用程序層能更好地被理解。

是否支援重定優先級 ( Reprioritisation ) 仍在討論中。 HTTP/2 具有優先級框架來處理此問題，但是 QUIC 和 HTTP/3 中串流真正的獨立使這一問題變得更加複雜，因此，此項目仍在討論中。

當（ 或如果 ）為 HTTP/3 商定了更好的優先級模型時，希望也能夠將該模型反向移植到 HTTP/2，以解決那裡的複雜性和實現問題。