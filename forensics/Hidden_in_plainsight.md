## Hidden in plainsight
Difficulty: Easy

### How I solved it

- opened my Linus VM

- downloaded the challenge file into the VM

- using basic commands to inspect the contents

<code>file <filename></code>
<code>strings <filename></code>

- noticed unusual pattern and should not be a normal file content

- using `grep` to search deeply

<code>strings <filename> | grep -i pico</code>

