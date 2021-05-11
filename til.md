# TIL

[Scala metals](https://scalameta.org/metals/) is configured through the
`JAVA_OPTS` environment variable, so it's easy to make wrapper scripts that
invoke metals with different configurations.  E.g. to change the bloop port,
run `JAVA_OPTS=-Dmetals.bloop-port=8124 metals`.

The default `escape-time` in TMUX makes it difficult to use programs where
hitting the Escape key happens frequently (such as Vim). To fix the problem,
set `escape-time` to a low number: `set -sg escape-time 30` in your
`~/.tmux.conf`.

The [Kurtosis](https://en.wikipedia.org/wiki/Kurtosis) of set of samples
describes the shape of the "tail" of the distribution - it's primarily
concerned with outliers. There are 2 different "types": Pearson's Kurtosis, and
Excess Kurtosis (aka. Fisher's Kurtosis), which is the former minus 3 to
account for the fact that the Pearson's Kurtosis of the normal distribution is
3. Kurtosis is the 4th standardized moment.

In the [NERDTree](https://github.com/preservim/nerdtree) Vim plugin, the
behaviour of opening a file explorer with the current file's location fully
expanded is accessed with the command `:NERDTreeFind`.

There is a [WebGL2](https://www.khronos.org/registry/webgl/specs/latest/2.0/)
which adds many features to the existing WebGL spec (e.g. instanced rendering).
It's supported by most browsers.

The `source` keyword in bash is not POSIX, but the dot (`.`) (which has the
same effect) is.

Compensated Summation algorithms (e.g. [Kahan Summation
Algorithm](https://en.wikipedia.org/wiki/Kahan_summation_algorithm)) are a class
of algorithms for computing the sum of a collection of numbers in more
numerically-stable way than naive addition, and can reduce the rounding errors
typical when adding a large amount of floating point number, or a collection of
floating point numbers where values vary in order of magnitude.

[Marks in Vim](https://vim.fandom.com/wiki/Using_marks) let you name locations
within a file for navigating to later. `ma` creates a mark named "a" at the
cursor position. `'a` moves the cursor to the line containing mark "a", and
`` `a `` moves the cursor to the precise location of mark "a".
