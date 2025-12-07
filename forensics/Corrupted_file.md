## Corrupted File
Difficulty: Easy

### How I solved it

- opened VM

- downloaded the file into VM

- used `file` to inspect the file type 

- used the hex view to inspect the file header

  `hexdump -C corrupted | head`

- compared the broken header with the correct magic bytes for the expected file type

- edited the file 

```
xxd corrupted > hex.txt
xxd -r hex.txt repaired_file
```
- opened the repaired file

  `xdg-open repaired_file`
