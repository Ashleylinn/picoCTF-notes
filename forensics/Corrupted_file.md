## Corrupted file
Difficulty: Easy

### How I solved it

- opened VM

- downloaded the file into VM

- used `file` to inspect the file type 

- used the hex view to inspect the file header

<code>hexdump -C corrupted | head</code>

- compared the broken header with the correct magic bytes for the expected file type

- edited the file 

<code>
xxd corrupted > hex.txt
xxd -r hex.txt repaired_file
</code>

- opened the repaired file

<code>xdg-open repaired_file</code>
