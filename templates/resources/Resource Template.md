---
Links: "[[My Resources]]"
---
---



<%* 
const DIRECTORY = "3 - resources/"
const BASE_NEW_FILENAME = "📕 Resource"

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
