Using Diuretic is usually as simple as adding an import, alongside another
project which implements
[Anticipation](https://github.com/propensive/anticipation/) typeclasses.
Currently six contextual imports are available for three different Anticipation
modules.

### Time Representation

Diuretic provides a choice of three different representations of durations and instants:

- `timeRepresentation.javaTime`—uses `java.time.Instant` for instants and
  `Long` for durations
- `timeRepresentation.javaLongTime`—uses `Long` for both instants and durations
- `timeRepresentation.javaUtil`—uses `java.util.Date` for instants and `Long`
  for durations

### File Representation

Diuretic provides a choice of two different file representations:

- `fileRepresentation.javaNio`—uses `java.nio.file.Path` for files, directories and paths
- `fileRepresentation.javaIo`—uses `java.io.File` for files, directories and paths

A possible future version may offer representations which use distinct types
for paths (which may not relate to a file or directory) and files/directories.

### URL Representation

- `urlRepresentation.javaNet`—uses `java.net.URL` for URLs