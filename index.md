---
layout: default
---

<body>
  <div class="index-wrapper">
    <div class="aside">
      <div class="info-card">
        <h1 style="font-size:60px;">Hua13</h1> 
        <a href="http://blog.csdn.net/qq_17280755/" target="_blank"><img src="http://blog.csdn.net/favicon.ico" alt="" width="25"/></a>
        <a href="https://www.douban.com/people/peihua13/" target="_blank"><img src="http://www.douban.com/favicon.ico" alt="" width="25"/></a>
        <a href="https://www.zhihu.com/people/peihua13/" target="_blank"><img src="https://www.zhihu.com/favicon.ico" alt="" width="25"/></a>
      </div>
      <div id="particles-js"></div>
    </div>

    <div class="index-content">
      <ul class="artical-list">
        {% for post in site.categories.blog %}
        <li>
          <a href="{{ post.url }}" class="title">{{ post.title }}</a>
          <div class="title-desc">{{ post.description }}</div>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
</body>
