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

# Unidata

```
CREATE-FILE DICT MVMAKE.BP 11

ED VOC MVMAKE.BP
1> DIR
2> /usr/local/mvappsvr/pkgs/mvmake/MVMAKE.BP
3> <leave as is>

ED VOC MVMAKE.BP.ROOT
1> DIR
2> /usr/local/mvappsvr/pkgs/mvmake
3> <SAME AS MVMAKE.BP>
```

```
# jBASE

ED MD MVMAMKE.BP
1>F
2>mvmake/MVMAKE.BP
3>mvmake
```



