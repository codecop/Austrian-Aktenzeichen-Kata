# Das Österreiche Aktenzeichen

Practice your object oriented design skills on the Austrian Aktenzeichen.

[Das Österreichische Aktenzeichen](https://de.wikipedia.org/wiki/Aktenzeichen_(%C3%96sterreich)) dient zur Identifikation Schriftstücken welche dieselbe Rechtssache betreffen und in einem Akt gesammelt und vereinigt werden. Es besteht aus dem Gattungszeichen, der Aktenzahl und der Jahresangabe. Wo gleichartige Sachen in mehreren Gerichtsabteilungen geführt werden, wird dem Gattungszeichen die der Abteilungszahl vorangestellt.

The Austrian Aktenzeichen is the reference number used in court cases in Austria,
similar to the US [case citation numbers](https://en.wikipedia.org/wiki/Case_citation) or
[European Case Law Identifier](https://en.wikipedia.org/wiki/European_Case_Law_Identifier).
It contains several numbers and identifiers combined into a single composite reference.
[Wikipedia's description](https://de.wikipedia.org/wiki/Aktenzeichen_(%C3%96sterreich)) is detailed.

## Analyse Requirements

* [Read Wikipedia](https://de.wikipedia.org/wiki/Aktenzeichen_(%C3%96sterreich)) (really!)
* Which elements are in the ref number?
* Which ones are mandatory/ optional?
* Which format does each part have?
* Numbers are usually not just `\d+`.
* Are there alternative options?
* Think about white space, separators, etc.

## Task

Write code to

* parse different String representations
* use internal, unified model
* output in different formats
* compare two ref numbers for equality
* ignore checksum for equality
* sort two ref numbers by creation time
* validate (calculate checksum)

## Reduced Requirements

At least create code for

* Model of Aktenzeichen including Gattungszeichen, Aktenzahl and Jahresangabe, e.g. `C420/05`.
* Comparison of two Aktenzeichen: `equals` and `compare`.
* Parse the Aktenzeichens.

## Design Considerations

* Immutability
* Encapsulation
* Composition over Inheritance
* SRP

### Design Hints/Spoilers

[1](https://www.martinfowler.com/bliki/ValueObject.html)
[2](https://sourcemaking.com/design_patterns/composite)
