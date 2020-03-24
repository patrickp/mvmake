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

# jBASE
```
ED MD MVMAMKE.BP
1>F
2>mvmake/MVMAKE.BP
3>mvmake
```

# Unidata
```
CREATE-FILE (DICT MVMAKE.BP
1>DIR
2>mvmake/MVMAKE.BP
3>D_MVMAKE.BP

SELECT * TO COMPILE
BASIC OFF LIST
CATALOG WITH FORCE TO NOT ASK QUESTIONS
```
# QM
```
QM looks to want the BP.OUT.  I think universe wants this also.

ED MVMAKE.BP
1>F
2>mvmake/MVMAKE.BP]MVMAKE.BP/BP.OUT
3>mvmake
4>MVMAKE.BP]BP.OUT
```




## Work
```
1/19/2020 4:18 - Need to adjust package to create q-pointers
1/19/2020 4:18 - Need Make Clean to remove items
1/21/2020 11:21AM - Told compiler to build F pointers the same as Universe.  Had to manually make into multi-part.
02/06/2020 07:38PM - Update mvmake to have compile.  This was actually just a git pull issue.
02/06/2020 07:39PM - Updated .gitignore with $!BASIC.OPTIONS
                     Added option to write out MV.PLATFORM.JSON if it does not exist
                     Added MVMAKE.QM
02/09/2020 01:12PM - Added d3 compile options.  Also adjust (dict to data.  Still need to test fsi accounts!
03/19/2020 12:24pm - Added universe compile/catalog items
                     


````



