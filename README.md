# iso-codes
This repository contains ISO-639-1 Language Code dictionaries. 

# Files
This is a description of the files in this repository
## [iso-codes.txt](https://github.com/theRealProHacker/iso-codes/blob/main/iso-codes.txt)
The source file which contains all the information. However, it might be quite cumbersome to parse it.

## [iso_simp.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso_simp.json)
This file contains a simple dictonary that puts the ISO-Codes directly in relation to the language name:  
`{language_code:language_name}`  

### [iso_simp.min.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso_simp.min.json)
This file is a minified version of the [iso_simp.json file](https://github.com/theRealProHacker/iso-codes/blob/main/iso_simp.json)  

## [iso_full.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso_full.json)  
This file contains a more complex dictionary that contains all information from the source in the following form:  
```json
{
  "language_code":
    {
      "language":"language_name",
      "family": "the language family",
      "x-info": "extra information"
    }
}
``` 

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
