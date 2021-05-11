# TIL

[Scala metals](https://scalameta.org/metals/) is configured through the
`JAVA_OPTS` environment variable, so it's easy to make wrapper scripts that
invoke metals with different configurations.  E.g. to change the bloop port,
run `JAVA_OPTS=-Dmetals.bloop-port=8124 metals`.

[Marks in VIM](https://vim.fandom.com/wiki/Using_marks) let you name locations
within a file for navigating to later. `ma` creates a mark named "a" at the
cursor position. `'a` moves the cursor to the line containing mark "a", and
`\`a` moves the cursor to the precise location of mark "a".
