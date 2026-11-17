# PS GAME STORE — WebKit Host

This is a visual rebrand of the user-provided `ufm42/wobkot` source. The original JS source files are preserved byte-for-byte, and the original `LICENSE.txt` remains included.

## Hosting on GitHub Pages

1. Extract this ZIP onto your PC.
2. Create a new public GitHub repository, e.g. `PS5-1360`.
3. Upload the *contents of the extracted folder*, not this ZIP. `index.html` and `src/` must be in the repository root.
4. GitHub repository → Settings → Pages → Build and deployment → Deploy from a branch → `main` and `/(root)` → Save.
5. Your example link is `https://USERNAME.github.io/PS5-1360/` (replace USERNAME).

## Important limitation

This upload contains **no** `src/ps5/elfldr.elf` and **no** `src/ps5/kexp.bin`. The upstream `README.md` requires both for PS5. The PS5 script explicitly fetches these files from `src/ps5/` after earlier execution stages. The published website is *not* proof that the exploit will work on 13.60.

Do not publish private SSL keys, credentials, personal files, or other secrets. The uploaded archive contained `localhost.pem` with a **private key** and certificate. Both `localhost.pem` and `host.py` have been omitted from this public-hosting version because GitHub Pages is static-only. `host.py` is not executable by GitHub Pages.

Do not distribute any extra binary payloads publicly unless you trust their source and have permission to distribute them. The original Git ignore rules exclude the payload filenames from version control.

The JavaScript files must not be changed casually: small changes can affect exploit reliability. The branding is isolated to `index.html`.

## Upstream

- Original project: https://github.com/ufm42/wobkot
- `README.md` and `LICENSE.txt` are from the uploaded upstream archive.
