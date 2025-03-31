---
course: <% tp.file.title.split("_")[0] %> <% tp.file.title.split("_")[1] %>
type: lecture
lecture_num: <% tp.file.title.split("_")[3] %>
date: <% tp.date.now("M/D") %>
---

# <% tp.file.title.split("_")[0] %> <% tp.file.title.split("_")[1] %> Lecture <% tp.file.title.split("_")[3] %>
- ## <% tp.date.now("M/D") %>

## Topic

- 

---

<%*
let num = Number(tp.file.title.split("_")[3]);
let prev = num > 1 ? `Previous: [BILD 3 Lecture ${num-1}](BILD_1_LE_${num-1}.md).` : "";
let next = num < 30 ? `Next: [BILD 3 Lecture ${num+1}](BILD_1_LE_${num+1}.md).` : "";
if (prev && next) {
    tR += prev + "\n" + next;
} else {
    tR += prev + next;
}
%>