# Find Copies

This bash script checks whether all files listed in the current directory
are to be found in the target directory structure.

File comparison is done via filename lookup, and then md5 comparison

## Usage

```
fc path/to/target/dir
```

Output

```
IMG_1178.JPG c6db682162b551044216cf0d097f8a3c vs c6db682162b551044216cf0d097f8a3c OK
IMG_1215.JPG bf9be225b76ce7b93f38ffb9772583b6 vs bf9be225b76ce7b93f38ffb9772583b6 OK
IMG_1216.JPG b2a1c576a7e6b4ce9b5fcf20935c7226 vs b2a1c5asdf79ds87fa096dfdsf760asd FAIL
```
