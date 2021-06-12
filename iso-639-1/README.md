# About
This folder contains the iso-639-1 language codes
## Files
This is a description of the files in this folder

## [iso-codes.txt](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso-codes.txt)
The source file which contains all the information. However, it might be quite cumbersome to parse it.

## [iso_simp.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_simp.json)
This file contains a simple dictonary that puts the ISO-Codes directly in relation to the language name:  
`{language_code:language_name}`  

### [iso_simp.min.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_simp.min.json)
This file is a minified version of the [iso_simp.json file](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_simp.json)  

## [iso_full.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_full.json)  
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

### [iso_full.min.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_full.min.json)
This is again the minified version of [iso_full.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_full.json)
