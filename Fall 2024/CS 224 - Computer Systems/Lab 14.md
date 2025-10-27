# 6.26

| Cache |  m  |  C   |  B  |  E  |  S  |  t  |  s  |  b  |
| :---: | :-: | :--: | :-: | :-: | :-: | :-: | :-: | :-: |
|   1   | 32  | 2048 |  8  |  1  | 256 | 21  |  8  |  3  |
|   2   | 32  | 2048 |  4  |  4  | 128 | 23  |  7  |  2  |
|   3   | 32  | 1024 |  2  |  8  | 64  | 25  |  6  |  1  |
|   4   | 32  | 1024 | 32  |  2  | 16  | 23  |  4  |  5  |
# 6.29
![[Pasted image 20241210112930.png]]
**A.**

| 12  | 11  | 10  |  9  |  8  |  7  |  6  |  5  |  4  |  3  |  2  |  1  |  0  |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| CT  | CT  | CT  | CT  | CT  | CT  | CT  | CT  | CT  | CI  | CI  | CO  | CO  |
**B.**

**0x834**

| 12  | 11  | 10  |  9  |  8  |  7  |  6  |  5  |  4  |  3  |  2  |  1  |  0  |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|  0  |  1  |  0  |  0  |  0  |  0  |  0  |  1  |  1  |  0  |  1  |  0  |  0  |
|  0  |  8  |  8  |  8  |  8  |  3  |  3  |  3  |  3  |  4  |  4  |  4  |  4  |
CT: 010000011 = 0x83
CI: 01 = 1
CB: 00 = 0

Cache miss

**0x836**

| 12  | 11  | 10  |  9  |  8  |  7  |  6  |  5  |  4  |  3  |  2  |  1  |  0  |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|  0  |  1  |  0  |  0  |  0  |  0  |  0  |  1  |  1  |  0  |  1  |  1  |  0  |
|  0  |  8  |  8  |  8  |  8  |  3  |  3  |  3  |  3  |  6  |  6  |  6  |  6  |
CT: 010000011 = 0x83
CI: 01 = 1
CB: 10 = 2

Cache miss

**0xFFD**

| 11  | 10  |  9  |  8  |  7  |  6  |  5  |  4  |  3  |  2  |  1  |  0  |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|  1  |  1  |  1  |  1  |  1  |  1  |  1  |  1  |  1  |  1  |  0  |  1  |
|  F  |  F  |  F  |  F  |  F  |  F  |  F  |  F  |  D  |  D  |  D  |  D  |

CT: 11111111 = 0xFF
CI: 11 = 3
CB: 01 = 1

Cache Hit: C0
# 6.36 
``` C
int x[2][128];
int i;

int sum = 0;

for (i = 0; i < 128; i++) {
	sum += x[0][i] * x[1][i]
}
```
![[Pasted image 20241209111854.png]]
**A. Case 1: Assume the cache is 512 bytes, direct-mapped, with 16 byte cache blocks. What is the miss rate?** 
100%

**B. Case 2: what is the miss rate if we double the cache size to 1024?**
25%

**C. Case 3: Now assume the cache is 512 bytes, two-way set associative using an LRU replacement policy, with 16-byte cache blocks. What is the cache miss rate?**
25%

**D. For case 3, will a larger cache size help to reduce the miss rate? Why or why not?**
No, we will still have the same number of cold misses

**E. For case 3, will a larger block size help to reduce the miss rate? Why or why not?**
Yes, you can load more from the array into the cache for each cold miss.
