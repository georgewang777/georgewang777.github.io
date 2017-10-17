---
layout: default
---

<body>
  <div class="index-wrapper">
    <div class="aside">
      <div class="info-card">
        <h1 style="font-size:100px;">Hua13</h1> 
        <a href="http://blog.csdn.net/qq_17280755/" target="_blank"><img src="http://blog.csdn.net/favicon.ico" alt="" width="28"/></a>
        <a href="https://www.douban.com/people/peihua13/" target="_blank"><img src="http://www.douban.com/favicon.ico" alt="" width="30"/></a>
        <a href="https://www.zhihu.com/people/peihua13/" target="_blank"><img src="https://www.zhihu.com/favicon.ico" alt="" width="30"/></a>
		<script type="text/javascript">
			var d = new Date();
			var time = d.getHours();
			if (time<10)
			{
				document.write("<p style="color: red;font-size: 300%;font-family: verdana">早上好</p>");
			}
			else if (time>=10 && time<16)
			{
				document.write("<p style="color: red;font-size: 300%;font-family: verdana">今天好</p>");
			}
			else
			{
				document.write("<p style="color: red;font-size: 300%;font-family: verdana">晚上好!</p>");
			}
		</script>
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
