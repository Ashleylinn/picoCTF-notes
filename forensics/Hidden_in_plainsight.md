## Hidden in Plainsight
Difficulty: Easy

### How I solved it:

- opened my Linus VM

- downloaded the challenge file into the VM

- using basic commands to inspect the contents

    `file <filename>`

    `strings <filename>`

- noticed unusual pattern and should not be a normal file content

- using `grep` to search deeply

    `strings <filename> | grep -i pico`

