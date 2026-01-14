---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## Welcome to Pinternship

**Pinternship by VLED Lab** — A comprehensive full-stack development internship program for mastering the MERN stack under the guidance of **Prof. Sudarshan Iyengar** at IIT Ropar's VLED Lab. Learn TypeScript, React, Express.js, and MongoDB through hands-on case studies and real-world projects.





## 📢 Announcements

{% assign announcements_page = site.pages | where: "permalink", "/announcements/" | first %}
{% for announcement in announcements_page.announcements limit:2 %}
{{ forloop.index }}. **[{{ announcement.title }}](./announcements/)** ({{ announcement.date }})  
   {{ announcement.description | truncatewords: 20 }}
{% endfor %}

➡️ [View All Announcements](./announcements/)