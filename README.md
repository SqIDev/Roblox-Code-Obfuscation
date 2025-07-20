Lua Binary Reversal Obfuscator

A simple educational Lua module for Roblox that demonstrates a symmetric data transformation by reversing a number's binary representation. This project is a great example of data manipulation and the importance of preserving data integrity.

About The Project

This script was created to explore a basic form of data obfuscation. It is not designed for real-world security but serves as an excellent educational tool. The core logic involves a three-step process:

1.  **Convert:** An integer is converted into its binary string representation.
2.  **Transform:** The binary string is reversed.
3.  **Revert:** The reversed binary string is converted back into a new integer.

A key challenge in this process is handling trailing zeros in the original binary, which become leading zeros after being reversed. These leading zeros are normally lost during number conversion. This script solves that problem by tracking the original `bitCount`, ensuring the transformation is perfectly reversible for any integer.

> ⚠️ **Warning:** This is an obfuscation method, not a cryptographic one. It is **not secure** and should only be used for educational or non-sensitive purposes.

Features

-   Transforms any integer into a new, obfuscated integer.
-   Perfectly reversible decryption process.
-   Correctly handles trailing/leading zeros by tracking the original bit count.
-   Written in a clean, reusable `ModuleScript` format.
-   Includes a `VirtualMachine` script with a full suite of automated tests.

How To Use

1.  Create a `Folder` in `ServerScriptService` (e.g., named `CodeObfuscator`).
2.  Place the `CodeExecutor` `ModuleScript` and the `VirtualMachine` `Script` inside that folder.
3.  Run the game. The `VirtualMachine` will automatically run and print the test results to the output.

### File Structure
▼ ServerScriptService
▼ CodeObfuscator (Folder)
🧱 CodeExecutor (ModuleScript)
📄 VirtualMachine (Script)

NOTE: This repository is related to my other repository called: 'Roblox-Code-Cryptography'.
The system is similar in terms of scripts used, the syntax is different, to serve a different objective.
