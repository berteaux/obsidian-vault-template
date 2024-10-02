---
tags:
  - output
Links: "[[My Outputs]]"
---

---
<%* 
const DIRECTORY = "0 - outputs/"
const BASE_NEW_FILENAME = "Output Note"

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