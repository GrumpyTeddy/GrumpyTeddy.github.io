---
title: 关于我
date: 2026-04-29T10:30:00+08:00
draft: false
type: about
featuredImage: /images/banner.jpg
markup:
  goldmark:
    renderer:
      unsafe: true
---

<div class="about-container">
    <div class="about-header">
        <img src="/images/avatar.jpg" alt="头像" class="about-avatar" />
        <h1 class="about-title">二哈</h1>
        <p class="about-subtitle">热爱技术的学习者</p>
    </div>
  
<div class="about-content">
    <div class="about-section">
      <h2 class="section-title">👤 个人简介</h2>
      <p class="section-text">
        大家好！我是二哈，一个热爱技术的学习者。我相信技术的力量，希望通过不断学习和实践，成为一名优秀的开发者。
      </p>
    </div>
    
<div class="about-section">
        <h2 class="section-title">🎓 背景信息</h2>
        <div class="info-grid">
        <div class="info-item">
          <div class="info-icon">🎓</div>
          <div class="info-content">
            <h3>学历</h3>
            <p>本2双非硕</p>
          </div>
        </div>
        <div class="info-item">
          <div class="info-icon">⏰</div>
          <div class="info-content">
            <h3>Gap</h3>
            <p>两年</p>
          </div>
        </div>
        <div class="info-item">
          <div class="info-icon">🚀</div>
          <div class="info-content">
            <h3>方向</h3>
            <p>AI和游戏引擎</p>
          </div>
        </div>
      </div>
    </div>
    
<div class="about-section">
      <h2 class="section-title">📚 学习方向</h2>
      <div class="learning-path">
        <div class="learning-card">
          <div class="card-icon">💻</div>
          <h3>C++</h3>
          <p>C++基础还可以，打算阅读《Effective C++》和《Effective STL》</p>
        </div>
        <div class="learning-card">
          <div class="card-icon">🎨</div>
          <h3>图形学</h3>
          <p>正在学习《Games101》第二遍，学习到了几何部分</p>
        </div>
        <div class="learning-card">
          <div class="card-icon">🤖</div>
          <h3>AI</h3>
          <p>目前相当于没有基础，打算按照这个路线学习：李沐 → CS224N → CS336</p>
        </div>
      </div>
    </div>
    
  <div class="about-section">
      <h2 class="section-title">🌟 技能树</h2>
      <div class="skill-tree">
        {{< mermaid >}}
        graph LR
          A[C++] --> B[图形学]
          A[C++] --> C[AI]
          B[图形学] --> D[游戏引擎]
          C[AI] --> E[深度学习] 
        {{< /mermaid >}}
      </div>
    </div>
    
<div class="about-section">
      <h2 class="section-title">📬 联系方式</h2>
      <div class="contact-grid">
        <a href="https://github.com/GrumpyTeddy" class="contact-item" target="_blank">
          <div class="contact-icon">🐙</div>
          <h3>GitHub</h3>
          <p>GrumpyTeddy</p>
        </a>
        <a href="mailto:moleyunfei@gmail.com" class="contact-item">
          <div class="contact-icon">📧</div>
          <h3>邮箱</h3>
          <p>moleyunfei@gmail.com</p>
        </a>
      </div>
    </div>
    
<div class="about-section">
      <h2 class="section-title">✨ 博客目的</h2>
      <p class="section-text">
        这个博客主要用于记录我从开始学习到找到第一份实习的心路历程，分享我的学习心得和技术成长。希望通过这个平台，与更多志同道合的朋友交流学习，共同进步！
      </p>
    </div>
  </div>
</div>

<style>
.about-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem;
}

.about-header {
  text-align: center;
  margin-bottom: 3rem;
}

.about-avatar {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 4px solid #ff6b6b;
  box-shadow: 0 4px 20px rgba(255, 107, 107, 0.3);
  margin-bottom: 1.5rem;
}

.about-title {
  font-size: 2.5rem;
  font-weight: bold;
  background: linear-gradient(135deg, #ff6b6b, #4ecdc4);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 0.5rem;
}

.about-subtitle {
  font-size: 1.2rem;
  color: #5a6c7d;
  margin: 0;
}

[data-theme=dark] .about-subtitle {
  color: #e8e8eb;
}

.about-content {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.about-section {
  background: linear-gradient(135deg, rgba(255, 228, 225, 0.3) 0%, rgba(255, 240, 245, 0.3) 50%, rgba(224, 255, 255, 0.3) 100%);
  border-radius: 1rem;
  padding: 2rem;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

[data-theme=dark] .about-section {
  background: linear-gradient(135deg, rgba(45, 55, 72, 0.5) 0%, rgba(61, 74, 90, 0.5) 50%, rgba(74, 85, 104, 0.5) 100%);
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
}

.section-title {
  font-size: 1.8rem;
  font-weight: bold;
  color: #ff6b6b;
  margin-bottom: 1rem;
}

[data-theme=dark] .section-title {
  color: #4ecdc4;
}

.section-text {
  font-size: 1.1rem;
  line-height: 1.8;
  color: #5a6c7d;
}

[data-theme=dark] .section-text {
  color: #e8e8eb;
}

.info-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
}

.info-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background: rgba(255, 255, 255, 0.5);
  border-radius: 0.5rem;
  transition: all 0.3s ease;
}

[data-theme=dark] .info-item {
  background: rgba(0, 0, 0, 0.3);
}

.info-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
}

.info-icon {
  font-size: 2.5rem;
}

.info-content h3 {
  font-size: 1.2rem;
  color: #ff6b6b;
  margin-bottom: 0.3rem;
}

[data-theme=dark] .info-content h3 {
  color: #4ecdc4;
}

.info-content p {
  font-size: 1rem;
  color: #5a6c7d;
  margin: 0;
}

[data-theme=dark] .info-content p {
  color: #e8e8eb;
}

.learning-path {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
}

.learning-card {
  background: linear-gradient(135deg, rgba(255, 107, 107, 0.1) 0%, rgba(78, 205, 196, 0.1) 100%);
  border: 2px solid rgba(255, 107, 107, 0.3);
  border-radius: 1rem;
  padding: 1.5rem;
  text-align: center;
  transition: all 0.3s ease;
}

[data-theme=dark] .learning-card {
  background: linear-gradient(135deg, rgba(78, 205, 196, 0.1) 0%, rgba(255, 107, 107, 0.1) 100%);
  border-color: rgba(78, 205, 196, 0.3);
}

.learning-card:hover {
  transform: translateY(-10px) scale(1.05);
  box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

.card-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.learning-card h3 {
  font-size: 1.5rem;
  color: #ff6b6b;
  margin-bottom: 0.5rem;
}

[data-theme=dark] .learning-card h3 {
  color: #4ecdc4;
}

.learning-card p {
  font-size: 1rem;
  color: #5a6c7d;
  line-height: 1.6;
}

[data-theme=dark] .learning-card p {
  color: #e8e8eb;
}

.skill-tree {
  background: rgba(255, 255, 255, 0.5);
  border-radius: 1rem;
  padding: 1.5rem;
  text-align: center;
}

[data-theme=dark] .skill-tree {
  background: rgba(0, 0, 0, 0.3);
}

.contact-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
}

.contact-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1.5rem;
  background: linear-gradient(135deg, rgba(255, 107, 107, 0.1) 0%, rgba(78, 205, 196, 0.1) 100%);
  border: 2px solid rgba(255, 107, 107, 0.3);
  border-radius: 1rem;
  text-decoration: none;
  transition: all 0.3s ease;
}

[data-theme=dark] .contact-item {
  background: linear-gradient(135deg, rgba(78, 205, 196, 0.1) 0%, rgba(255, 107, 107, 0.1) 100%);
  border-color: rgba(78, 205, 196, 0.3);
}

.contact-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 20px rgba(255, 107, 107, 0.4);
}

.contact-icon {
  font-size: 2.5rem;
}

.contact-item h3 {
  font-size: 1.2rem;
  color: #ff6b6b;
  margin-bottom: 0.3rem;
}

[data-theme=dark] .contact-item h3 {
  color: #4ecdc4;
}

.contact-item p {
  font-size: 1rem;
  color: #5a6c7d;
  margin: 0;
}

[data-theme=dark] .contact-item p {
  color: #e8e8eb;
}

@media (max-width: 768px) {
  .about-container {
    padding: 1rem;
  }
  
  .about-title {
    font-size: 2rem;
  }
  
  .info-grid,
  .learning-path,
  .contact-grid {
    grid-template-columns: 1fr;
  }
}
</style>