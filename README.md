# iso-codes
This repository contains ISO-639-1 Language Code dictionaries. 

### [iso_full.min.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso_full.min.json)
This is again the minified version of [iso_full.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso_full.json)

# Usage
A short python example to use this dictionary instead of pycountry for example  
To do this you have to put the iso_simp.min.json file into your filesystem with the python script  
```python
  import json #the advantage is that you have no new dependencies
  get_language_as_iso_code():
    #some function that returns an ISO-Code like for example from langid, langdetect, fastText or nltk
    return "en"
  with open("iso_simp.min.json","r") as file:
    iso_codes=json.load(file)
  myISOCode=get_language_as_iso_code()
  print(iso_codes[myISOCode]) #-> "english"
```
