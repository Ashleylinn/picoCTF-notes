## DISKO 1
Difficulty: Easy

### How I solved it

- I only use two steps to find the flag
- `gunzip disko-1.dd.gz` then it becomes a disko-1.dd file
- then i use `strings disko-1.dd | grep -i pico` to find a specifc word
- then found the flag
