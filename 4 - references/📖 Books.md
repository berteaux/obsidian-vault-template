---
tags:
  - reference
Links: "[[My References]]"
Status:
  - status/todo
---

---

```dataview
LIST
FROM #reference  AND !"templates"
WHERE contains(Links, [[]])
SORT file.name
```

