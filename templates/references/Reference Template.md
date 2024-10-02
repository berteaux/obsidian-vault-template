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

<%* 
const DIRECTORY = "4 - references/"
const BASE_NEW_FILENAME = "📖 Reference"

let id = 1;
let filename = BASE_NEW_FILENAME;
while (await tp.file.exists(DIRECTORY + filename + ".md")) {
	filename = BASE_NEW_FILENAME + " " + id;
	id++
}

const NEW_PATH = DIRECTORY + filename
await tp.file.rename(filename) 
await tp.file.move(NEW_PATH)
-%>