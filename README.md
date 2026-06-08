# Homework 7

This project is configured to work offline using local libraries in the `lib/` directory. All code resides in the default package.

## 📂 Project Structure

```
h7/
├── src/main/java/       # Application source code
│   └── Huffman.java
├── src/test/java/       # Test code
│   ├── HuffmanTest.java
│   └── Aout.java        # Test helper utilities
├── lib/                 # Local libraries
│   ├── junit-4.13.2.jar
│   └── hamcrest-core-1.3.jar
├── bin/                 # Compiled class files
└──
```

## 🛠️ Command Line Instructions

Since the project uses the default package and local JAR files, commands differ by operating system (path separator: Windows `;` vs Linux/Mac `:`).

### Windows (Command Prompt / PowerShell)

```bash
# 1. Compile main code
javac -d bin src/main/java/*.java

# 2. Compile tests (requires lib folder and main code in bin)
javac -d bin -cp "lib/*;bin" src/test/java/*.java

# 3. Run application
java -cp bin Huffman

# 4. Run JUnit tests
java -cp "bin;lib/*" org.junit.runner.JUnitCore HuffmanTest
```

### Linux and macOS

```bash
# 1. Compile main code
javac -d bin src/main/java/*.java

# 2. Compile tests (requires lib folder and main code in bin)
javac -d bin -cp "lib/*:bin" src/test/java/*.java

# 3. Run application
java -cp bin Huffman

# 4. Run JUnit tests
java -cp "bin:lib/*" org.junit.runner.JUnitCore HuffmanTest
```

---

## 📋 Task Description

Write a constructor to create a Huffman prefix code for a given byte array and
 methods to encode and decode the data. The code must be optimal and decoding
 must restore the original array.
 Do not forget to test the byte array of length one.
Example API is at: https://enos.itcollege.ee/~japoia/algoritmid/kodeerimisyl.html 
If any sources are used provide the references.


Koostada meetodid Huffmani prefikskoodi loomiseks etteantud baitmassiivi põhjal
 (konstruktorina), selle baitmassiivi kodeerimiseks ning kodeeritud massiivi
 dekodeerimiseks. Kontrollitakse koodi optimaalsust ning kodeeriva ja dekodeeriva
 meetodi kooskõlalisust. Kodeeritav massiiv võib koosneda ka ühestainsast baidist
 (testige see juhtum eraldi).
API näidise leiate: https://enos.itcollege.ee/~japoia/algoritmid/kodeerimisyl.html
Allikad tuleb viidata.

---

## ⚙️ Requirements

- **Java 8** or higher
