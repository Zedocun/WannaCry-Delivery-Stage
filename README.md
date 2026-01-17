## WannaCry - Password-Protected Delivery Stage

This repository documents an early stage analysis of a WannaCry sample that embeds an encrypted ZIP archive inside a Windows PE executable.

### Key Observations
* The file presents as a valid PE executable.
* Static inspection reveals a PK ZIP archive marked as encrypted.
* High entropy suggests compressed or encrypted embedded content.
* A hardcoded string within the binary enables archive extraction.
* Extracted content contains known WannaCry components.

### Scope
This project focuses strictly on the **delivery and pre-execution stage**.
Execution flow, encryption routines, and propagation are intentionally out of scope.

### Disclaimer
No malware binaries, passwords, payloads, or extraction instructions are included.
This repository is intended for educational and analytical purposes only.
