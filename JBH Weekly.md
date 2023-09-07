---
summary: 
week: <% tp.date.now("YYYY-[W]W", 0, tp.file.title, "YYYY-[W]W") %>
year: <% tp.date.now("YYYY", 0, tp.file.title, "YYYY-[W]W") %>
tags:
  - weekly
---
# Notes
***

# History
***

<%*
Array.from(Array(7).keys()).map((i) => {
  date = tp.date.weekday("YYYY-MM-DD", i, tp.file.title, "YYYY-[W]W");
  tR += `### ${date}\n`;
  tR += `![[Notes/${date}#Outcomes]]\n\n`;
});
%>
