---
author: "{% if authorUrl %} [{{author}}]({{authorUrl}}) {% elif author %} [[{{author}}]] {% endif %}"
"Amazon Link:": "{% if url %}[{{% title %}}]({{url}}){% endif %}"
kindle link: "{% if appLink %}[Kindle link]({{appLink}}){% endif %}"
pages: "{% if pages %}{{pages}}{% endif %}"
year: "{% if publicationDate %} {{ publicationDate }} {% endif %}"
last annotation date: "{{ lastAnnotatedDate }}"
asin: "{% if asin %}{{asin}}{% endif %}"
isbn: "{% if isbn %}{{isbn}}{% endif %}"
tags:
  - kindleSync
  - book
  - automation
  - sync
---
```
{{authorsLastNames}} - {{title}}

---
title: "{{title}}"
{% trim %}
author: "{{author}}"
amazon link: "{{url}}"
kindle link: "{{appLink}}"
pages: "{{pages}}"
publication: "{{publication}}"
publisher: "{{publisher}}"
asin: "{{asin}}"
isbn: "{{isbn}}"
{% endtrim %}
tags:
  - kindleSync
  - book
  - automation
  - sync
---

# Notes & Highlights
***

{{highlights}}


> [!quote] Location: [{{ location }}]({{ appLink }})
> {{ text }} 
> {{ createdDate }} 

{% if note %}
>[!sticky] Note:
>{{note}}
{% endif %}

***

```