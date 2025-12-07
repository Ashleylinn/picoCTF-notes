## Riddle Registry
Difficulty: Easy 

### How I Solved it 

- inspect the file using `exiftool`

- the author field has a Base64 string in metadata

- decoded with `base64 -d`