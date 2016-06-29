# Find/Compare Duplicates/Missing Files

This bash script checks whether all files listed in the current directory
are to be found in the target directory structure.

File comparison is done via filename lookup, and then md5 comparison

## Usage

```
fc path/to/target/dir
```

Output

```

IMG_0924.JPG MISSING

IMG_0925.JPG MISSING

IMG_1013.JPG d39758c23d0ee3ffd4312dff0f67bb14 vs aba843ea31411ea5a711447fc4e04d47 ../../PhotoLibrary//2005/04/15/img_1013.jpg FAIL
IMG_1013.JPG d39758c23d0ee3ffd4312dff0f67bb14 vs 1bbe4ec290abccf77b4b287a471ac563 ../../PhotoLibrary//2009/09/19/img_1013.jpg FAIL
IMG_1013.JPG d39758c23d0ee3ffd4312dff0f67bb14 vs 5ac8d0097b53648ac0bb7440af9ce20b ../../PhotoLibrary//2013/12/22/IMG_1013.jpg FAIL
IMG_1013.JPG d39758c23d0ee3ffd4312dff0f67bb14 vs d39758c23d0ee3ffd4312dff0f67bb14 ../../PhotoLibrary//2016/04/06/IMG_1013.JPG OK

IMG_1014.JPG 7f18e55d3fd93baec18c1e2779e3435f vs 6255a48429cf5ab0a3c20e76cdf5f11b ../../PhotoLibrary//2005/04/15/img_1014.jpg FAIL
IMG_1014.JPG 7f18e55d3fd93baec18c1e2779e3435f vs 2eaafef96953f6dc6e52a81475cc3cd2 ../../PhotoLibrary//2009/09/19/img_1014.jpg FAIL
IMG_1014.JPG 7f18e55d3fd93baec18c1e2779e3435f vs d61463924089154e4e0424fd1a72a4eb ../../PhotoLibrary//2013/12/22/IMG_1014.jpg FAIL
IMG_1014.JPG 7f18e55d3fd93baec18c1e2779e3435f vs 7f18e55d3fd93baec18c1e2779e3435f ../../PhotoLibrary//2016/04/06/IMG_1014.JPG OK

```
