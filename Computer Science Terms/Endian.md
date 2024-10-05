#computer-science #bytes #memory #machine-code
# Little Endian vs Big Endian

Little and Big Endian are methods of byte ordering used by operation systems. Little Endian stores values in memory from least significant bits to most significant bits. Big Endian is the inverse. 

If we want to store the value `0xAB` (171 in decimal) at a given memory location

| Style          | Values       |
| -------------- | ------------ |
| Human Readable | `0xAB`       |
| Little Endian  | `[0xB, 0xA]` |
| Big Endian     | `[0xA, 0xB]` |
