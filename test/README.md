# SVG-cleaner test files

next files have different content but must same rendered on screen

+ `svg-cleaner.svg` - svg test file
![IN](svg-cleaner.svg)
+ `svg-cleaned.svg` - optimized svg file
![OUT](svg-cleaned.svg)

# SVG-cleaner test

    svg-cleaner.test - simple test checked equal by `md5sum`

output

```
[i] RUN ../svg-cleaner svg-cleaner.svg > /tmp/svg-cleaner-tests/svg-cleaned.svg
[i] IN svg-cleaner.svg OUT &STDOUT
 The initial file size is 14997 bytes
 The initial number of elements is 105
 The initial number of attributes is 294

 The final file size is 5533 bytes
 The final number of elements is 27
 The final number of attributes is 86

 The new file size is 36.89%
 The number of removed elements is 78
 The number of removed attributes is 208

[i] svg-cleaner.svg (18276) => /tmp/svg-cleaner-tests/svg-cleaned.svg (5566)
svg-cleaned.svg: OK
svg-cleaner.svg: OK
```
