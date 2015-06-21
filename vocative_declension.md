# Declension of names to vocative case

Goals:

- automatical declension of names to the vocative case
    - for greeting
    - names can be composed of multiple parts and quite complex
- estimating gender from the name
- normalization of the name
    - eg. from all lower/upper case to the canonical form
- adding missing diacritics
- working correctly with lowercase and upper case letters
- applicable to languages:
    - Czech
    - ???
- greeting by title:
    - eg. `MUDr. Novák` -> `pane doktore Nováku`
- auto-complete
- web service
- pure front-end service (just a JS)
- batch processing - for mailing lists

## Implementation

- posible solutions:
    - rule-based
    - based on machine-learning

- http://github.com/bzamecnik/salutr
    - port of http://www.pteryx.net/sklonovani.html
    - completely refactored
    - just vocative case
    - added possibility of declining complex names
    - rule-based
    - Scala, JavaScript
    - web service
    - batch mode - CSV input/output
    - open-source

### Gotchas

- composed surnames: `Schaumburg-Lippe`
- middle names: `František Xaver Šalda`
- foreign names
- no title case: McArthur
- additional charachters: O'Hara
- names with various structure, eg. asian names vs. european names
    - european: given name, middle name, family name
    - asian: family name, middle name, given name
- gender-ambiguous names
    - the name name could be either male or female

### Useful

- name surname statistics in Czech republic
    - http://www.mvcr.cz/clanek/cetnost-jmen-a-prijmeni-722752.aspx?q=Y2hudW09MQ%3D%3D

##  Similar projects

- [České skloňování / The czech declensions](http://www.pteryx.net/sklonovani.html) - Pavel Sedlák (Pteryx)
    - general rules-based Czech declension in all cases and both numbers
    - a prototype made by an amateur
    - (-) horrible code, no API
    - JavaScript
    - (+) open-source
- http://www.sklonovani-prijmeni.cz/
    - (-) done by hand + using some internal software
    - (-) not a web service
    - (-) paid
    - (-) just surnames
- Lingea
    - (-) C library
    - (-) paid
    - (+) possibly very good
