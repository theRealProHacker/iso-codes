# iso-codes
This repository contains ISO-639-1 and ISO-639-3 Language Code dictionaries. 

# Usage
A short python example to use this dictionary instead of pycountry for example  
To do this you have to put the iso_simp.min.json file into your filesystem with the python script  
```python
  import json #the advantage is that you have no new dependencies
  get_language_as_iso_code():
    #some function that returns an ISO-639-1-Code
    return "en"
  with open("iso_simp.min.json","r") as file:
    iso_codes=json.load(file)
  myISOCode=get_language_as_iso_code()
  print(iso_codes[myISOCode]) #-> "english"
```
