# Regex Tagesschulung

## Beispiele

#### Eine Zahl größer 15:
    \b(?:1[6-9]|[2-9]\d|\d{3,})\b
    \b(?:1(?:[6-9]|\d{2,})|[2-9]\d+)\b

#### Eine Zeichenkette mit gerader Länge:
    \b(?:.{2})+\b

#### Eine Zeile welche error,ERROR,Error,etc enhält:
    /^.*error.*$/mgi

#### Ein korrektes Datum:
    \d{2}\.\d{2}\.\d{4}
    (0[1-9]|[1-2][0-9]|3[0-1])\.(0[1-9]|1[0-2])\.(\d{4}) 

#### Alle Sätze welche mit einem ! enden:
    (?<=[\.\!\?] )(?:[\w\s]+)(?=!)

#### Hexadezimal Color Code:
    #(?:[0-9a-fA-F]{3}){1,2}

#### Numbers:
    ^[+-]?(0)?(?(1)|[1-9]\d+)(\.|,)?(?(2)\d+)$

#### Passwörter (mind. 8 Zeichen , Zumindest: zwei Kleinbuchstaben, zwei Großbuchstaben, 2 Zahlen, ein Sonderzeichen):
    ^(?=.*[A-Z].*[A-Z])(?=.*\d.*\d)(?=.*[a-z].*[a-z])(?=.*[.&%$!_\-]).{8,}$
