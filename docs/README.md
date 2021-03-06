
> @hexlet/fs@0.3.8 documentation /home/stas/Work/hexlet/hexlet-components/js-fs
> documentation "build" "src/index.js" "-f" "md"

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [index][1]
    -   [Examples][2]
    -   [mkdirSync][3]
        -   [Parameters][4]
        -   [Examples][5]
    -   [mkdirpSync][6]
        -   [Parameters][7]
        -   [Examples][8]
    -   [rmdirSync][9]
        -   [Parameters][10]
        -   [Examples][11]
    -   [touchSync][12]
        -   [Parameters][13]
        -   [Examples][14]
    -   [unlinkSync][15]
        -   [Parameters][16]
        -   [Examples][17]
    -   [readdirSync][18]
        -   [Parameters][19]
        -   [Examples][20]
    -   [statSync][21]
        -   [Parameters][22]
        -   [Examples][23]
    -   [writeFileSync][24]
        -   [Parameters][25]
        -   [Examples][26]
    -   [readFileSync][27]
        -   [Parameters][28]
        -   [Examples][29]
    -   [copySync][30]
        -   [Parameters][31]
-   [Dir][32]
    -   [Parameters][33]
    -   [Examples][34]
    -   [isDirectory][35]
        -   [Examples][36]
    -   [isFile][37]
        -   [Examples][38]
-   [Node][39]
    -   [Parameters][40]
    -   [getStats][41]
    -   [getName][42]
-   [Stats][43]
    -   [Parameters][44]
    -   [isFile][45]
    -   [isDirectory][46]
-   [File][47]
    -   [Parameters][48]
    -   [Examples][49]
    -   [getBody][50]
        -   [Examples][51]
    -   [isDirectory][52]
        -   [Examples][53]
    -   [isFile][54]
        -   [Examples][55]
-   [constructor][56]
    -   [Parameters][57]

## index

Make FS

### Examples

```javascript
const fs = new HexletFs();
```

### mkdirSync

Make directory

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.mkdirSync('/opt');
```

### mkdirpSync

Make directory

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.mkdirpSync('/etc/nginx/conf.d');
```

### rmdirSync

Remove directory

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.rmdirSync('/opt');
```

### touchSync

Touch file

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.touchSync('/etc/nginx/nginx.conf');
fs.touchSync('/etc/hosts');
```

### unlinkSync

Unlink file

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.unlinkSync('/etc/nginx/nginx.conf');
```

### readdirSync

Read directory

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.readdirSync('/etc'); // ['nginx', 'hosts']
```

### statSync

Get file stat

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.statSync('/etc/hosts').isFile(); // true
fs.statSync('/etc').isDirectory(); // true
```

### writeFileSync

Write file

#### Parameters

-   `filepath`  
-   `body`  

#### Examples

```javascript
fs.writeFileSync('/etc/hosts', 'localhost');
```

### readFileSync

Read file

#### Parameters

-   `filepath`  

#### Examples

```javascript
fs.readFileSync('/etc/hosts'); // 'localhost'
```

### copySync

Copy file
fs.copySync('/etc/hosts', '/etc/nginx');
fs.readdirSync('/etc/nginx'); // [ 'conf.d', 'hosts' ]

#### Parameters

-   `src`  
-   `dest`  

## Dir

**Extends Node**

Directory

### Parameters

-   `name`  

### Examples

```javascript
const dir = new Dir('/');
```

### isDirectory

Returns true if it's a file system directory.

#### Examples

```javascript
const dir = new Dir('/');
dir.isDirectory(); // true
```

### isFile

Returns false if it's a file system directory.

#### Examples

```javascript
const dir = new Dir('/');
dir.isFile(); // false
```

## Node

File

### Parameters

-   `name`  

### getStats

Get stats

### getName

Get name

## Stats

Stats

### Parameters

-   `file`  
-   `directory`  

### isFile

is file?

### isDirectory

is directory?

## File

**Extends Node**

File

### Parameters

-   `name`  
-   `body`  

### Examples

```javascript
const file = new File('file.txt', 'body');
```

### getBody

Get file's body

#### Examples

```javascript
const file = new File('file.txt', 'body');
file.getBody(); // 'body'
```

### isDirectory

Returns false if it's a regular file.

#### Examples

```javascript
const file = new File('file.txt', 'body');
file.isDirectory(); // false
```

### isFile

Returns true if it's a regular file.

#### Examples

```javascript
const file = new File('file.txt', 'body');
file.isFile(); // true
```

## constructor

Constructor

### Parameters

-   `error`  
-   `path`  

[1]: #index

[2]: #examples

[3]: #mkdirsync

[4]: #parameters

[5]: #examples-1

[6]: #mkdirpsync

[7]: #parameters-1

[8]: #examples-2

[9]: #rmdirsync

[10]: #parameters-2

[11]: #examples-3

[12]: #touchsync

[13]: #parameters-3

[14]: #examples-4

[15]: #unlinksync

[16]: #parameters-4

[17]: #examples-5

[18]: #readdirsync

[19]: #parameters-5

[20]: #examples-6

[21]: #statsync

[22]: #parameters-6

[23]: #examples-7

[24]: #writefilesync

[25]: #parameters-7

[26]: #examples-8

[27]: #readfilesync

[28]: #parameters-8

[29]: #examples-9

[30]: #copysync

[31]: #parameters-9

[32]: #dir

[33]: #parameters-10

[34]: #examples-10

[35]: #isdirectory

[36]: #examples-11

[37]: #isfile

[38]: #examples-12

[39]: #node

[40]: #parameters-11

[41]: #getstats

[42]: #getname

[43]: #stats

[44]: #parameters-12

[45]: #isfile-1

[46]: #isdirectory-1

[47]: #file

[48]: #parameters-13

[49]: #examples-13

[50]: #getbody

[51]: #examples-14

[52]: #isdirectory-2

[53]: #examples-15

[54]: #isfile-2

[55]: #examples-16

[56]: #constructor

[57]: #parameters-14
