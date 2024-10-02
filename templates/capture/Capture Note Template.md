---
tags:
  - capture/note
Status:
  - status/todo
Date: <% tp.file.creation_date() %>
Links: "[[My Captures]]"
---

---
<%* 
const DIRECTORY = "0 - capture/"
const BASE_NEW_FILENAME = "Capture Note"

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