WebP Express 0.15.3. Conversion triggered using bulk conversion, 2019-09-24 05:34:53

*WebP Convert 2.1.4*  ignited.
- PHP version: 7.3.1
- Server software: Apache

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2015/08/image2xxl-92.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image2xxl-92.jpg.webp
- log-call-arguments: true
- converters: (array of 9 items)

The following options have not been explicitly set, so using the following defaults:
- converter-options: (empty array)
- shuffle: false
- preferred-converters: (empty array)
- extra-converters: (empty array)

The following options were supplied and are passed on to the converters in the stack:
- default-quality: 70
- encoding: "auto"
- max-quality: 80
- metadata: "none"
- near-lossless: 60
- quality: "auto"
------------


*Trying: cwebp* 

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2015/08/image2xxl-92.jpg
- destination: [doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image2xxl-92.jpg.webp
- default-quality: 70
- encoding: "auto"
- low-memory: true
- log-call-arguments: true
- max-quality: 80
- metadata: "none"
- method: 6
- near-lossless: 60
- quality: "auto"
- use-nice: true
- command-line-options: ""
- try-common-system-paths: true
- try-supplied-binary-for-os: true

The following options have not been explicitly set, so using the following defaults:
- alpha-quality: 85
- auto-filter: false
- preset: "none"
- size-in-percentage: null (not set)
- skip: false
- rel-path-to-precompiled-binaries: *****
------------

Encoding is set to auto - converting to both lossless and lossy and selecting the smallest file

Converting to lossy
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Quality of source is 92. This is higher than max-quality, so using max-quality instead (80)
The near-lossless option ignored for lossy
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -m 6 -low_memory '[doc-root]/wp-content/uploads/2015/08/image2xxl-92.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image2xxl-92.jpg.webp.lossy.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image2xxl-92.jpg.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2015/08/image2xxl-92.jpg
Dimension: 870 x 1110
Output:    50554 bytes Y-U-V-All-PSNR 41.97 48.86 48.61   43.29 dB
           (0.42 bpp)
block count:  intra4:       1734  (45.04%)
              intra16:      2116  (54.96%)
              skipped:      1056  (27.43%)
bytes used:  header:            181  (0.4%)
             mode-partition:   8514  (16.8%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |   32739 |     803 |     978 |     264 |   34784  (68.8%)
 intra16-coeffs:  |     980 |     263 |     706 |    1023 |    2972  (5.9%)
  chroma coeffs:  |    3448 |     106 |     209 |     311 |    4074  (8.1%)
    macroblocks:  |      34%|       5%|       9%|      52%|    3850
      quantizer:  |      27 |      23 |      18 |      13 |
   filter level:  |      18 |      20 |      17 |      16 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |   37167 |    1172 |    1893 |    1598 |   41830  (82.7%)

Success
Reduction: 67% (went from 149 kb to 49 kb)

Converting to lossless
Locating cwebp binaries
1 cwebp binaries found in common system locations
Checking if we have a supplied binary for OS: Darwin... We do.
We in fact have 1
A total of 2 cwebp binaries where found
Detecting versions of the cwebp binaries found (and verifying that they can be executed in the process)
Executing: /usr/local/bin/cwebp -version. Result: version: 1.0.3
Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12 -version
Exec failed (the cwebp binary was not found at path: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-mac12)
Trying executing the cwebs found until success. Starting with the ones with highest version number.
Creating command line options for version: 1.0.3
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata none -q 80 -alpha_q '85' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2015/08/image2xxl-92.jpg' -o '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image2xxl-92.jpg.webp.lossless.webp' 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/webp-express/webp-images/doc-root/wp-content/uploads/2015/08/image2xxl-92.jpg.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2015/08/image2xxl-92.jpg
Dimension: 870 x 1110
Output:    353650 bytes (2.93 bpp)
Lossless-ARGB compressed size: 353650 bytes
  * Header size: 4469 bytes, image data size: 349156
  * Lossless features used: PREDICTION CROSS-COLOR-TRANSFORM SUBTRACT-GREEN
  * Precision Bits: histogram=5 transform=4 cache=10

Success
Reduction: -132% (went from 149 kb to 345 kb)

Picking lossy
cwebp succeeded :)

Converted image in 1491 ms, reducing file size with 67% (went from 149 kb to 49 kb)
