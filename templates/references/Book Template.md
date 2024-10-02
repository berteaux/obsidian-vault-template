---
tags:
  - reference/book
Links: "[[📖 Books]]"
Resources: 
Status:
  - status/todo
---
---

[Write Table of Contents and try to summary each point]

___
References:
- 

<%* 
const DIRECTORY = "notes/"
const BASE_NEW_FILENAME = "Book Reference"

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