---
layout: page
title: 嚴選服務
permalink: /product/
---

<div class="market-container">
  <!-- 嚴選賣場連結 -->
  <a class="market-item" href="https://shopee.tw/your-shop-url1" target="_blank" class="market-link">
    <img src="{{ '/source/img/fotor-ai-product01.jpg' | relative_url }}" alt="嚴選賣場" style="max-width: 200px; height: auto;">
    <div class="overlay">
      <span class="title">嚴選賣場</span>
    </div>
  </a>

  <!-- 茶品賣場連結 -->
  <a class="market-item" href="https://shopee.tw/your-shop-url2" target="_blank" class="market-link">
    <img src="{{ '/assets/img/tea.png' | relative_url }}" alt="茶品賣場" style="max-width: 200px; height: auto;">
    <div class="overlay">
      <span class="title">茶品賣場</span>
    </div>
  </a>
</div>

<!-- 頁面獨立的配置 -->
<style>
.market-container {
  display: flex;
  gap: 15px; /* 調整項目之間的間距 */
}

.market-link {
  position: relative;
  display: inline-block; /* 讓圖片的外部容器適當包裹圖片 */
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(255, 255, 255, 0.7); /* 半透明白色 */
  display: flex;
  justify-content: center; /* 垂直置中 */
  align-items: center; /* 水平置中 */
  opacity: 0; /* 初始透明 */
  transition: opacity 0.3s ease; /* 透明度過渡效果 */
}

.market-link:hover .overlay {
  opacity: 1; /* 懸停時顯示 */
}

.title {
  font-size: 16px; /* 標題字體大小 */
  font-weight: bold; /* 字體加粗 */
  color: #333; /* 標題顏色 */
}
</style>
