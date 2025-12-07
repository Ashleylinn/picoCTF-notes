## Flag in Flame
Difficulty: Easy

### How I solved it

- opened VM

- donwloaded the file into VM

- checked the file type `file Logs.txt`

- inspected using `less` and the file contained many block of encoded text (likely base64)

- decoded the file using `base64 -d Logs.txt > output.txt`

- then `cat output.txt` to see the output


