# WAN-IFRA-BarCode
## The 16-digit bar code WAN-IFRA
### (Symbology: Interleaved 2/5)
(modifications approved by the IFRA Newsprint Commitee on October 1, 1991)

| Offset | Lenght | Description
|:------:|:------:|------------
|      1 |    8   | [Reel number](#reel-number) ([Scandinavian manufacturer](#scandinavian-manufacturer)) ([Central European manufacturer](#central-european-manufacturer))
|      9 |    4   | Reel weight
|     13 |    1   | [Copacking](#copacking) + [Manufacturer code](#manufacturer-code)
|     14 |    1   | [Grammage and quality](#grammage-and-quality)
|     15 |    2   | [Manufacturer code](#manufacturer-code)

## Reel number
### Scandinavian manufacturer

| Offset | Lenght | Description
|:------:|:------:|------------
|      1 |    1   | Paper machine number
|      2 |    2   | Week of manufacture
|      4 |    5   | Serial number (<50000 even years, >49999 uneven years)

### Central European manufacturer

| Offset | Lenght | Description
|:------:|:------:|------------
|      1 |    1   | Paper machine number
|      2 |    2   | Week of manufacture
|      4 |    3   | Tambour number (<500 even years, >499 uneven years)
|      7 |    1   | Set from tambour
|      8 |    1   | Position in tambour

## Copacking
If digit 13 is odd number (1, 3, 5 or 7): 1 reel per wrapping

If digit 13 is even number (2, 4, 6 or 8): 2 reel per wrapping


## Grammage and quality

| Value | Description
|:-----:|-------------
|   1   | 40 g/m² standard newsprint
|   2   | 45 g/m² standard newsprint
|   3   | 48.8 g/m² standard newsprint
|   4   | 52 g/m² standard newsprint
|   5   | Other standard newsprint
|   6   | 45 g/m² upgraded newsprint
|   7   | 48.8 g/m² upgraded newsprint
|   8   | 52 g/m² upgraded newsprint
|   9   | 55 g/m² upgraded newsprint
|   0   | Other

## Manufacturer code

Digit 13: Manufacturer list
Digits 15 and 16: Manufacturer code

| Digit 13 | Manufacturer list
|:--------:|------------------
|  1 or 2  | [List 1](Manufacturers%20list%201.md)
|  3 or 4  | [List 2](Manufacturers%20list%202.md)
|  5 or 6  | [List 3](Manufacturers%20list%203.md)
