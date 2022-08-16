# Decompiling Project Zomboid
Example repository demonstrating how to decompile the Project Zomboid source for use in mod development.

This example is entirely based on the (excellent) [documentation by konjima](https://github.com/Konijima/PZ-Libraries) on
how to structure a IntelliJ IDEA project, configure Gradle, and run the decompiler. As someone who struggled with
using some of the tooling initially, I can't express my appreciation for this documentation enough.


## Getting Started
Run configurations are already generated. Run the `setupWorkspace` Gradle task to get started.

See the [Decompiling section](https://github.com/Konijima/PZ-Libraries#c-decompiling) of the documentation.


## Additional Tasks
Several Gradle tasks will be added to assist with storing and versioning the generated artifacts in `lib`:

| Task | Description | Status     |
| ---- | ----------- |------------|
| `createSourceDirectory` | create a directory to store generated source files in. | Incomplete |
| `createCurrentVersionDirectory` | create a subdirectory for source files for the current Zomboid version. | Incomplete |
| `copySourceFiles` | copy contents of `lib` to sources directory. | Incomplete |
| `removeCurrentVersionDirectory` | remove sources from sources directory for current Zomboid version, if any exist. | Incomplete |
        

## References

- [Capsid](https://github.com/pzstorm/capsid): Capsid is a compact mod development environment for Project Zomboid.

- [ZomboidDoc](https://github.com/cocolabs/pz-zdoc): ZomboidDoc is a Lua library compiler for Project Zomboid.

- [ZomboidMod](https://github.com/cocolabs/pz-zmod): ZomboidMod is compact mod development environment for Project Zomboid.

- [EmmyLua](https://emmylua.github.io/?plugin): Support for Lua programming language in [IntelliJ IDEA](https://www.jetbrains.com/idea).

- [Gradle](https://gradle.org/)