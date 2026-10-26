# Security policy

## Reporting a vulnerability

Please **don't open a public issue** for security problems.

Report them privately through GitHub: on this repository's **Security** tab,
click **Report a vulnerability**
([direct link](https://github.com/namshubs/hypersuite/security/advisories/new)).
Only the maintainer sees the report.

Please include:

- the hypersuite version (`hypersuite --version`),
- what an attacker could do, and under which conditions,
- steps or a file to reproduce it, if you have them.

You'll get an answer as soon as possible. Fixes are published as a new
release; the advisory is made public once a fixed version is available.

## Supported versions

Only the latest release receives fixes.

## Scope

hypersuite runs locally and makes no network connections. Of most interest
are problems where processing a crafted file (a PST, PDF, image, audio or
document file found during a scan) could run code, write outside the chosen
target, or delete or corrupt user data.

The bundled third-party tools (Tesseract, PDFium, fpcalc and their libraries)
are updated with hypersuite releases; for vulnerabilities in those projects
themselves, please also inform their maintainers.

## Verifying downloads

Every release lists SHA-256 checksums in `SHA256SUMS.txt`, and
`hypersuite.exe` is signed with the certificate `CN=hypersuite (github.com/namshubs/hypersuite)`
(thumbprint `C7EC126C59C0081863A4467F960C367BA1630C0D`). Don't run a
copy whose checksum or signature doesn't match.
