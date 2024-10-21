---
layout: page
title: 合作夥伴
permalink: /Partners/
published: false
---

<div class="market-container">
  <!-- 嚴選賣場連結 -->
  <a class="market-item" href="https://maps.app.goo.gl/rokNyRsif88P5NNw8" target="_blank" class="market-link">
    <img src="{{ '/source/img/partners/futchen.jpg' | relative_url }}" alt="賦成實業有限公司" style="max-width: 100px; height: auto;">
    <div class="overlay">
      <span class="title">賦成實業有限公司</span>
    </div>
  </a>
  <div class="partner-description">
    <p>賦成實業有限公司專注於提供工程設備租賃及人力派遣服務，擁有受傳承的豐富經驗與卓越的專業技術，致力於確保每一個案場順利且高效率地完成目標。</p>
  </div>
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
