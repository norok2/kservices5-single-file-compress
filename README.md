# kservices5-single-file-compress

## Installation

0. Obtain the appropriate utilities: `gzip`, `bzip2`, `lzip`, `xz`, `rzip`, `lrzip`.
1. Locate the *kservices* directory for KDE menu services using:
    `kf5-config --path services`;
    this is typically: `$HOME/.local/share/kservices5/` (local user) or `/usr/share/kservices5/` (system-wide)
2. Copy all `*.desktop` files to the desired *kservices* directory.
3. *Optional*: Register `rzip` mime-type
    1. Locate the *mime-type* directory; this is typically: `$HOME/.local/share/mime/` (local user) or `/usr/share/mime/` (system-wide)
    2. Copy `user-extension-rzip.xml` to the `packages` subdirectory within the desired *mime-type* directory.
    3. Run `update-mime <MIME-DIR>` (where `<MIME-DIR>` is the *mime-type* directory); may require root privileges for system-wide installation: use `su` or `sudo` as appropriate.

