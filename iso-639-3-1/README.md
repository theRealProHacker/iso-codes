# Converting From ISO639-3 To ISO639-1

This folder contains a json file that assigns all ISO639-1 codes to ISO639-3 codes.

`{iso-639-3:iso-639-1}`

## How to use

An example in python how to get the maximum from this dictionary. Before you do this put the file into your filesystem.

```python
#python
import json
with open("iso-639-3-1.json","r") as file:
  iso3_to_1=json.load(file)
#get an iso-1 code from an iso-3 code
try:
  print(iso3_to_1["eng"])#->"en"
except KeyError:
  print("The ISO639-3 code doesn't have an equivalent in ISO639-1")
#get an iso-3 code from an iso-1 code
iso1_to_3 = {v: k for k, v in iso3_to_1.items()}
print(iso1_to_3["en"])#->"eng"
#You normally don't need to except a KeyError if there is no user input
```
