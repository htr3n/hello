# hello

Demonstrate a bug with IntelliJ IDEA when handling importing of a Maven project that 
contains a file `pom.xml` and some other files prefixed with `pom.xml`, for instance,
`pom.xml.backup`, `pom.xml.tmp`, `pom.xml.old`, etc. Instead of picking the correct
`pom.xml`, IntelliJ IDEA tries to pick up all `pom.xml*` and creates multiple 
corresponding modules, namely, `xxx.iml`, `xxx (1).iml`, etc.
