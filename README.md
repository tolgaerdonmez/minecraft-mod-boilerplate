<h1 align="center">Welcome to minecraft-mod-boilerplate 👋</h1>
<p>
  <a href="https://twitter.com/tolgaerdonmez" target="_blank">
    <img alt="Twitter: tolgaerdonmez" src="https://img.shields.io/twitter/follow/tolgaerdonmez.svg?style=social" />
  </a>
</p>

> My Minecraft Forge Mod Boilerplate

> Minecraft version 1.16.1 (see build.gradle for further info)

## First to do before anything

> **modid** must be unique

Change `modid` everywhere and the com.tolgaerdonmez.dkmix everywhere you find, to your own
`dkmix` was modid, the convention is

`com.<yourname>.<modid>`

## Usage on VSCode

1. Install the Java Extension Pack
2. Open the project folder, vscode should automatically load the binaries
3. Run vscode runs from gradle tab > Gradle Tasks > fg_runs > runVSCodeRuns

### If you're using macOS also do these

1. Open the .vscode/launch.json
2. In the `runClient` object
3. Add `preLaunchTask:"purge-dsstore"`

## Starting Minecraft Client

Run the `runClient` in vscode **Run** panel. This will launch your mod attached to a minecraft instance

## Some part of official Forge MDK Readme

See the Forge Documentation online for more detailed instructions:
http://mcforge.readthedocs.io/en/latest/gettingstarted/

Step 1: Open your command-line and browse to the folder where you extracted the zip file.

Step 2: You're left with a choice.
If you prefer to use Eclipse:

1. Run the following command: "gradlew genEclipseRuns" (./gradlew genEclipseRuns if you are on Mac/Linux)
2. Open Eclipse, Import > Existing Gradle Project > Select Folder
   or run "gradlew eclipse" to generate the project.
   (Current Issue)
3. Open Project > Run/Debug Settings > Edit runClient and runServer > Environment
4. Edit MOD_CLASSES to show [modid]%%[Path]; 2 times rather then the generated 4.

If you prefer to use IntelliJ:

1. Open IDEA, and import project.
2. Select your build.gradle file and have it import.
3. Run the following command: "gradlew genIntellijRuns" (./gradlew genIntellijRuns if you are on Mac/Linux)
4. Refresh the Gradle Project in IDEA if required.

If at any point you are missing libraries in your IDE, or you've run into problems you can run "gradlew --refresh-dependencies" to refresh the local cache. "gradlew clean" to reset everything {this does not affect your code} and then start the processs again.

## Forge source installation

MinecraftForge ships with this code and installs it as part of the forge
installation process, no further action is required on your part.

## Author

👤 **Tolga Erdönmez**

-   Website: tidible.app
-   Twitter: [@tolgaerdonmez](https://twitter.com/tolgaerdonmez)
-   Github: [@tolgaerdonmez](https://github.com/tolgaerdonmez)
-   LinkedIn: [@tolgaerdonmez](https://linkedin.com/in/tolgaerdonmez)

## Show your support

Give a ⭐️ if this project helped you!

---

_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
