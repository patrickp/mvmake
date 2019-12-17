# MVMake

Cross Platform tool for creating Q-Pointers and building code

* jBASE,QM, Universe, Unidata - Create F-pointer
* D3 - Create d3 dictionary file.  Create Q pointer data section.

* root - Pointer to package/. This is primary for D3, but do the same on other platforms
* Other data sections, F/Q pointer to data Section.

* Code differences - Inline Inserts

* Platform specific code, create Q-pointer <package>.BP.INCLUDE, point to <package>.mvtype

An include is then

INCLUDE PACKAGE.BP.INCLUCE <include>

