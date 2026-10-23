# AutoPlay AI — Minecraft 1.21.11

A Fabric client-side experimental AutoPlay / training prototype. This repository is configured for Java 21 and Minecraft 1.21.11.

## Build

GitHub Actions builds the project on pushes and pull requests. You can also build locally with JDK 21 and Gradle 9.7.1:

```bash
gradle build
```

If the build succeeds, the mod JAR will be in `build/libs/`.

## Source layout

- `src/client/java/com/autoplay/AutoPlayClient.java` — main client mod source.
- `src/main/resources/fabric.mod.json` — Fabric metadata.
- `.github/workflows/build.yml` — GitHub Actions build workflow.

## Important

This is an experimental source package, not a verified release. The source uses Minecraft intermediary class/method names and has not been successfully compiled against the exact Minecraft 1.21.11 dependencies in this environment. Check the Actions log before treating the generated JAR as usable. Use automation only in single-player or on servers where it is explicitly permitted.
