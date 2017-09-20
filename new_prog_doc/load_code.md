Loading the robot code into your IDE
---

* auto-gen TOC:
{:toc}

## Common instructions
1. Open a terminal
2. `cd` to the folder where the code lives with `gradlew.bat` (or `gradlew` for Unix-likes)
3. Proceed to the instructions for your IDE.


## Idea/IntelliJ
3. Depending on your OS:
 * Windows: `gradlew.bat idea`
 * Unix-like (Linux, BSD, OSX?): `./gradlew idea` (you may have to do `chmod +x gradlew` first)
4. Once the task finishes, open IntelliJ.
5. Click "Import Project"
6. Browse to the `build.gradle` file in the popup, select it and click Ok.
7. Leave the Gradle settings in the next dialog alone unless you know what you're doing.
8. Let IntelliJ open the project, have much rejoicing. You're done!

## Eclipse

3. Depending on your OS:
 * Windows: `gradlew.bat eclipse`
 * Unix-like (Linux, BSD, OSX?): `./gradlew eclipse` (you may have to do `chmod +x gradlew` first)
4. Open Eclipse.
5. Pick any workspace directory you like.
6. Once Eclipse launches, go to File -> Open Projects from File System
7. Click the "Directory" button.
8. Find the folder that where `build.gradle` lives, and choose it.
9. Click finish, and wait for the import to finish. You're done.

**N.B.:** Eclipse has a different code formatting standard than IntelliJ. You **must** change the code formatting settings to match the IntelliJ defaults, which essentially amounts to using four spaces instead of a tab character.

We can have the tabs vs. spaces debate later, but for the time being we use spaces here. 

