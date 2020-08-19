---
permalink: /
title: "Hui Liu"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hui Liu received his Ph.D. in computer science in 2008 from the School of EECS of [Peking University ](http://english.pku.edu.cn/)under the direction of Professor Weizhong Shao. After graduation, he works as a teacher in [Beijing Institute of Technology](http://english.bit.edu.cn/). His research interests are in the area of software refactoring, software evolution, and software engineering. He and his research group is developing approaches and software tools to help software engineers to improve software quality by locating poorly designed source code fragments, and recommending easy restructuration (refactorings).

Research Interests
======
1. Smart IDE (智能化软件开发环境) 

2. Data Mining Based Software Engineering (基于数据挖掘的软件工程)

3. Software Maintenance and Evolution (软件维护与演化) 

4. Software Engineering (软件工程)

News
======
1. 课题组论文被[the 38th International Conference on Software Engineering](http://2016.icse.cs.txstate.edu/) (ICSE)录用。ICSE是中国计算机学会推荐的国际顶级A类会议（2015/12/18）。

{% capture written_year %}'None'{% endcapture %}

{% for post in site.posts %}

  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}

  {% if year != written_year %}

​    <h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>

​    {% capture written_year %}{{ year }}{% endcapture %}

  {% endif %}

  {% include archive-single.html %}

{% endfor %}