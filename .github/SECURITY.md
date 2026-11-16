# Security policy

## Supported versions

Only the [latest release](https://github.com/FiTH-g1gGLe/GamingTweaks/releases/latest) receives fixes.

## Reporting a problem

If you find something in GamingTweaks that could put a PC or its data at risk — for example a tweak that
weakens security in a way the README doesn't explain, or a download that isn't from an official source —
please **don't open a public issue**. Instead, use GitHub's private reporting:

**[Report a vulnerability](https://github.com/FiTH-g1gGLe/GamingTweaks/security/advisories/new)**

Include the GamingTweaks version, your Windows version and the log from `C:\GamingTweaks` if you can.
You'll get a reply as soon as possible, and a fix will be released with credit to you (unless you'd rather stay anonymous).

## Verifying a download

Every release is built by GitHub Actions directly from this repository, and its notes list the
SHA-256 checksum of `GamingTweaks.zip`. To check your download, open PowerShell in the folder and run:

```powershell
Get-FileHash .\GamingTweaks.zip -Algorithm SHA256
```

The value should match the one in the release notes. Only download GamingTweaks from
**github.com/FiTH-g1gGLe/GamingTweaks** — copies hosted anywhere else are not official.
