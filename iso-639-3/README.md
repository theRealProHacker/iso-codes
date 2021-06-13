# About

This folder contains the iso-639-3 language codes

## Files

This is a description of the files in this folder

## [iso_simp.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-3/iso_simp.json)

This file contains a simple dictonary that puts the ISO-Codes directly in relation to the language name:
`{language_code:language_name}`

### [iso_simp.min.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-3/iso_simp.min.json)

This file is a minified version of the [iso_simp.json file](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_simp.json). Normally this is what you will need most of the times

## [iso_full.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_full.json)

This file contains a more complex dictionary that contains extra information in the following form:

```json
{
  "language_code":
    {
      "name":"language_name",
      "type": "[living|historical|extinct|ancient|constructed|special]",
      "scope": "[individual|macrolanguage|special]"
    }
}
```

### [iso_full.min.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_full.min.json)

This is again the minified version of [iso_full.json](https://github.com/theRealProHacker/iso-codes/blob/main/iso-639-1/iso_full.json)
