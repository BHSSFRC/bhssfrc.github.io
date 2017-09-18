Loading the robot code into your IDE
---

* auto-gen TOC:
{:toc}

## Idea/IntelliJ
1. Open a terminal
2. `cd` to the folder where the code lives with `gradlew.bat` (or `gradlew` for Unix-likes)
3. Depending on your OS:
 * Windows: `gradlew.bat idea`
 * Unix-like (Linux, BSD, OSX?): `./gradlew idea` (you may have to do `chmod +x gradlew` first)
4. Once the task finishes, open IntelliJ.
5. Click "Import Project"
6. Browse to the `build.gradle` file in the popup, select it and click Ok.
7. Leave the Gradle settings in the next dialog alone unless you know what you're doing.
8. Let IntelliJ open the project, have much rejoicing. You're done!
