# iso-codes
This repository contains ISO-639-1 and ISO-639-3 Language Code dictionaries. 

# Usage
A short python code example with iso_simp.min in the iso-639-1 folder.  
To do this you have to put the iso_simp.min.json file into your filesystem with the python script  
```python
  import json #the advantage is that you have no new dependencies
  def get_language_as_iso_code():
    #some function that returns an ISO-639-1-Code
    return "en"
  with open("iso_simp.min.json","r") as file:
    iso_codes=json.load(file)
  myISOCode=get_language_as_iso_code()
  print(iso_codes[myISOCode]) #-> "english"
```

Another example in JavaScript  
```js
  function get_language_as_iso_code(){
    return "en"
  }
  let iso_codes=require("iso_simp.min.json")
  let myISOCode=get_language_as_iso()
  console.log(iso_codes[myISOCode])
```
