
### File Identification & Inspection 

- Check file types 

  ```
  file <filename>
  ```
- Print all readable text in a file
  ```
  strings <filename>
  ```
- View file contents page-by-page
  ```
  less <filename>
  ```
- View hex dump (inspect bytes)
  ```
  xxd <filename> | head
  hexdump -C <filename> | head
  ```

### Encoding & Decoding

(when seeing weird unusual text or content)

- Base64 decode
  ```
  base64 -d input.txt
  ```
- Base64 encode
  ```
  base64 input.txt
  ```
- ROT13 decode
  ```
  echo "text" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
  ```
- Hex → ASCII
  ```
  echo <hexstring> | xxd -r -p
  ```

### Searching & Filtering (Logs, large files)

- Search for keywords (case-insensitive)
  ```
  grep -i "keyword" filename
  ```
- Search recursively in folders
  ```
  grep -R "keyword" .
  ```
- Count occurrences
  ```
  grep -c "keyword" file
  ```
- Sort + unique (find unusual patterns)
  ```
  sort file | uniq -c | sort -nr
  ```

### Metadata Extraction

(useful for PDFs, images, audio, videos)

- Extract metadata
  ```
  exiftool <filename>
  ```
- Alternative
  ```
  strings <filename> | grep -i author
  ```


### Compression & Archive Handling

- Unzip
  ```
  unzip file.zip
  ```
- Tar extract
  ```
  tar -xvf archive.tar
  ```
- Gzip / gunzip
  ```
  gunzip file.gz
  ```

### Hashing (Identify checksums, verify integrity)

```
md5sum file
sha1sum file
sha256sum file
```

### Permissions & Execution Essentials

- Add execute permission
  ```
  chmod +x file
  ```
- Run a binary
  ```
  ./file
  ```

### Strings + Grep 

```
strings suspicious_file | grep -i pico
```

### Networking (Basic)

- Download file
  ```
  wget <url>
  curl -O <url>
  ```
- Send HTTP request
  ```
  curl http://example.com
  ```


### Virtual Machines

- Update VM packages
  ```
  sudo apt update
  sudo apt install <package>
  ```
- Tools should install
  ```
  sudo apt install exiftool
  sudo apt install binwalk
  sudo apt install foremost
  sudo apt install strings
  sudo apt install xxd
  ```

