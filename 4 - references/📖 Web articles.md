---
tags:
  - reference
Links: "[[My References]]"
---

---

```dataview
LIST
FROM #reference  AND !"templates"
WHERE contains(Links, [[]])
SORT file.name
```

