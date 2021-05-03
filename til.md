# TIL

[Scala metals](https://scalameta.org/metals/) is configured through the `JAVA_OPTS` environment
variable, so it's easy to make wrapper scripts that invoke metals with different configurations.
E.g. to change the bloop port, run `JAVA_OPTS=-Dmetals.bloop-port=8124 metals`.
