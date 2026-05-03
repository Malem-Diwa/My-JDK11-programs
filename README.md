I made all these Java programs in Termux using Ubuntu proot-distro. With Open Java Development Kit 11.
If you can not run the jar files, then: Install OpenJDK 11.
You can get OpenJDK 11 in the Eclipse Temurin site,
or if the link is dead. Go to this backup site: [https://mega.nz/folder/iYNylZ7a#HcfsP3vxM466JOLmXZQ2Fw]
Original Repo name:"JDK11-Everyday-programs" (Historical purpose only)

## REQUIREMENTS
- Java Development Kit 11 or Later Installed.
- *"java"* command available in the Terminal.
- Git installed.

## Build and Run

1. First, clone the repo with git:
```bash
git clone https://github.com/Malem-Diwa/My-JDK11-programs.git
```

2. Second, open the repository folder and go to A program folder:
```bash
cd "<folder>"
```

3. Third, Compile it to **Bytecode**:
```bash
javac *.java
```
This will produce .class files

4. Fourth, make your own MANIFEST.MF file. Point it to the class that contains `public static void main(java.lang.String[] args)` (Either your own modified code or my code.)
REMEMBER THAT MANIFEST.MF MUST CONTAIN: `Main-Class: classname` (And the class should have `public static void main(java.lang.String[] args)`

5. Fifth, package it to A jar: (OPTIONAL)
```bash
jar -cfm "<pkgname>.jar" "<yourmanifestfile>.mf" "*.class"
```

6. Sixth, run it: (OBVIOUSLY OPTIONAL)

> jar
```bash
java -jar "<pkgname>.jar"
```

> class
```bash
java classname
```

**CONGRATULATIONS!** That is it.

## Purpose?

NOT MUCH! I added this Repository because I love Open-Source Software.
That does not mean I dislike Proprietary Software (Not all Software must be *Open-Source*, right?), it just means I get more satisfaction seeing a Open-Source Software **MORE** than proprietary Software.
I am still fine with Proprietary Software.

## Notes
- In your Manifest file, point it to the class that contains `public static void main(java.lang.String[] args)`
- If you decide to run the Class directly instead of packaging it first, run the Class that has `public static void main(java.lang.String[] args)`
