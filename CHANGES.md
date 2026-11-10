# Changes for Paper 26.3

- `pom.xml`: Lamp 4.0.0-rc.12 → 4.0.1. The bundled Lamp read "26.3.build.237" as a version number and threw `NumberFormatException: "build"` in `BukkitVersion`, which is the `ExceptionInInitializerError` from issue #63. Lamp fixed the parser in June 2026.
- `pom.xml`: Kotlin 2.0.20 → 2.2.20. Kotlin 2.0.20 can't parse the Java 25 version string, so it couldn't compile on the JDK Paper 26.x needs. The bytecode target stays Java 21.
